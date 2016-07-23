# apigee-okta-integration
Apigee/Okta Integration: Resource Owner / Password Grant Flow in Action

Sample Requests:

Access Token Request (Token minted in Apigee):

curl -X POST  -d 'grant_type=password&user={{okta_user}}&password={{okta_password}}&client_id={{client_id}}&client_secret={{client_secret}}' "https://{{org}}-{{env}}.apigee.net/oauth-ext/token"

Access Token Request (Token minted externally):

curl -X POST  -d 'grant_type=password&user={{okta_user}}&password={{okta_password}}&client_id={{client_id}}' "https://{{org}}-{{env}}.apigee.net/oauth-ext2/token"

