# Qobuz Auth
OSS is no longer allowed to make use of the Qobuz api due to reports of abuse; use the following information at your own risk.

### Authorization tokes
The Qobuz REST api uses a different auth system than the standard Oauth method. 

Most (?) endpoints require `X-User-Auth-Token` and `X-App-Id` headers.  
While the `FileUrl` endpoint requires a Request Signature, formed from `format_id`, `track_id`, `timestamp`, and `app_secret` concatenated and md5 signed.
