// Sketchy loading of the jsrsasign library into Postman Sandbox
var navigator = {}; //fake a navigator object for the lib
var window = {}; //fake a window object for the lib
eval(pm.globals.get("jsrsasign-js")); //import javascript jsrsasign

var currentTime = +new Date(); // the current time in milliseconds
var issuedAtTimeSeconds = currentTime/1000;
var expirationTimeSeconds = currentTime/1000 + 3600;

// Grab the JWK from the Environment and change to JSON object
// The contents of the JWK variable should be the Public JWK only
var jwk = JSON.parse(pm.environment.get("jwk"));

// Generate random string for "jti" claim - needed if client has Replay Prevention enabled
var newJti="";
var charset = "abcdefghijklmnopqrstuvwxyz0123456789";

for( var i=0; i < 12; i++ ) {
    newJti += charset.charAt(Math.floor(Math.random() * charset.length));
}

pm.variables.set("jti", newJti);

// Create Header and Payload objects
var header = {
  "kid": jwk.kid,
  "alg": jwk.alg
};

var payload = {
  "iss": pm.environment.get("client_credentials_jwt"),
  "aud": "https://"+pm.environment.get("pingfed")+"/as/token.oauth2",
  "sub": pm.environment.get("client_credentials_jwt"),
  "jti": pm.variables.get("jti"),
  "exp" : Math.ceil(expirationTimeSeconds),
  "iat" : Math.ceil(issuedAtTimeSeconds)
};

// Prep the objects for a JWT
var sHeader = JSON.stringify(header);
var sPayload = JSON.stringify(payload);

var jwk = JSON.parse(pm.environment.get("jwk"));
var prvKey = KEYUTIL.getKey(jwk);

var sJWT = KJUR.jws.JWS.sign(header.alg, sHeader, sPayload, prvKey);

pm.environment.set("client_assertion", sJWT);
