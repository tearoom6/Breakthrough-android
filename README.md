# Breakthrough (Android)

[Memory Game] Breakthrough Android Project.

Released at [Google Play](https://play.google.com/store/apps/details?id=jp.tearoom6.MemoryTouch).

## Environments

- Unity 5.4.1
- fastlane 1.105.2 (gradle / supply)

## Configurations

Add configuration files for build (these files are added to .gitignore):

> gradle.properties

```
RELEASE_STORE_FILE=<KEYSTORE_FILE_PATH>
RELEASE_STORE_PASSWORD=<KEYSTORE_PASSWORD>
RELEASE_KEY_ALIAS=<KEY_ALIAS>
RELEASE_KEY_PASSWORD=<KEY_PASSWORD>
```

> local.properties

```
sdk.dir=<ANDROID_SDK_HOME>
```

> .secrets/Google\ Play\ Android\ Developer-4100b5eb7914.json (referenced from fastlane/Appfile)

```json
{
  "type": "service_account",
  "project_id": "<PROJECT_ID>",
  "private_key_id": "<PRIVATE_KEY_ID>",
  "private_key": "-----BEGIN PRIVATE KEY-----\n<ENCODED_PRIVATE_KEY>\n-----END PRIVATE KEY-----\n",
  "client_email": "<CLIENT_EMAIL>",
  "client_id": "<CLIENT_ID>",
  "auth_uri": "https://accounts.google.com/o/oauth2/auth",
  "token_uri": "https://accounts.google.com/o/oauth2/token",
  "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
  "client_x509_cert_url": "<CLIENT_X509_CERT_URL>"
}
```

