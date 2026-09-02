# AuthApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**acceptInvite**](AuthApi.md#acceptInvite) | **POST** /auth/accept-invite | Accept an invite: create the account (or reuse an existing one) and join the inviting tenant. The invite token proves control of the mailbox. |
| [**forgotPassword**](AuthApi.md#forgotPassword) | **POST** /auth/forgot-password | Send a password reset email to the user |
| [**login**](AuthApi.md#login) | **POST** /auth/login | Authenticate a user with email + password (optional TOTP) |
| [**logout**](AuthApi.md#logout) | **POST** /auth/logout | Log out the current user (kills the assay session) |
| [**magicLinkLogin**](AuthApi.md#magicLinkLogin) | **POST** /auth/magic-link | Request a magic link login (sends an email with a one-time link) |
| [**magicLinkVerify**](AuthApi.md#magicLinkVerify) | **POST** /auth/magic-link/verify | Verify a magic link token and log the user in |
| [**register**](AuthApi.md#register) | **POST** /auth/register | Register a new user account |
| [**resetPassword**](AuthApi.md#resetPassword) | **POST** /auth/reset-password | Reset the user&#39;s password using a reset token |
| [**totpEnable**](AuthApi.md#totpEnable) | **POST** /auth/totp/enable | Enable TOTP two-factor authentication by verifying a code |
| [**totpSetup**](AuthApi.md#totpSetup) | **GET** /auth/totp/setup | Set up TOTP two-factor authentication (generates secret + backup codes) |
| [**verifyEmail**](AuthApi.md#verifyEmail) | **POST** /auth/verify-email | Verify a user&#39;s email address using a verification token |


<a id="acceptInvite"></a>
# **acceptInvite**
> acceptInvite(acceptInviteRequest)

Accept an invite: create the account (or reuse an existing one) and join the inviting tenant. The invite token proves control of the mailbox.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
val acceptInviteRequest : AcceptInviteRequest =  // AcceptInviteRequest | 
try {
    apiInstance.acceptInvite(acceptInviteRequest)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#acceptInvite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#acceptInvite")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **acceptInviteRequest** | [**AcceptInviteRequest**](AcceptInviteRequest.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="forgotPassword"></a>
# **forgotPassword**
> forgotPassword(forgotPasswordRequest)

Send a password reset email to the user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
val forgotPasswordRequest : ForgotPasswordRequest =  // ForgotPasswordRequest | 
try {
    apiInstance.forgotPassword(forgotPasswordRequest)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#forgotPassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#forgotPassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **forgotPasswordRequest** | [**ForgotPasswordRequest**](ForgotPasswordRequest.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="login"></a>
# **login**
> AuthResponse login(loginRequest)

Authenticate a user with email + password (optional TOTP)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
val loginRequest : LoginRequest =  // LoginRequest | 
try {
    val result : AuthResponse = apiInstance.login(loginRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#login")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#login")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **loginRequest** | [**LoginRequest**](LoginRequest.md)|  | |

### Return type

[**AuthResponse**](AuthResponse.md)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="logout"></a>
# **logout**
> logout()

Log out the current user (kills the assay session)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
try {
    apiInstance.logout()
} catch (e: ClientException) {
    println("4xx response calling AuthApi#logout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#logout")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="magicLinkLogin"></a>
# **magicLinkLogin**
> magicLinkLogin(magicLinkRequest)

Request a magic link login (sends an email with a one-time link)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
val magicLinkRequest : MagicLinkRequest =  // MagicLinkRequest | 
try {
    apiInstance.magicLinkLogin(magicLinkRequest)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#magicLinkLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#magicLinkLogin")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **magicLinkRequest** | [**MagicLinkRequest**](MagicLinkRequest.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="magicLinkVerify"></a>
# **magicLinkVerify**
> AuthResponse magicLinkVerify(magicLinkVerifyRequest)

Verify a magic link token and log the user in

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
val magicLinkVerifyRequest : MagicLinkVerifyRequest =  // MagicLinkVerifyRequest | 
try {
    val result : AuthResponse = apiInstance.magicLinkVerify(magicLinkVerifyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#magicLinkVerify")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#magicLinkVerify")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **magicLinkVerifyRequest** | [**MagicLinkVerifyRequest**](MagicLinkVerifyRequest.md)|  | |

### Return type

[**AuthResponse**](AuthResponse.md)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="register"></a>
# **register**
> AuthResponse register(registerRequest)

Register a new user account

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
val registerRequest : RegisterRequest =  // RegisterRequest | 
try {
    val result : AuthResponse = apiInstance.register(registerRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#register")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#register")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **registerRequest** | [**RegisterRequest**](RegisterRequest.md)|  | |

### Return type

[**AuthResponse**](AuthResponse.md)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="resetPassword"></a>
# **resetPassword**
> resetPassword(resetPasswordRequest)

Reset the user&#39;s password using a reset token

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
val resetPasswordRequest : ResetPasswordRequest =  // ResetPasswordRequest | 
try {
    apiInstance.resetPassword(resetPasswordRequest)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#resetPassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#resetPassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **resetPasswordRequest** | [**ResetPasswordRequest**](ResetPasswordRequest.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="totpEnable"></a>
# **totpEnable**
> totpEnable(totpEnableRequest)

Enable TOTP two-factor authentication by verifying a code

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
val totpEnableRequest : TotpEnableRequest =  // TotpEnableRequest | 
try {
    apiInstance.totpEnable(totpEnableRequest)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#totpEnable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#totpEnable")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **totpEnableRequest** | [**TotpEnableRequest**](TotpEnableRequest.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="totpSetup"></a>
# **totpSetup**
> TotpSetupResponse totpSetup()

Set up TOTP two-factor authentication (generates secret + backup codes)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
try {
    val result : TotpSetupResponse = apiInstance.totpSetup()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#totpSetup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#totpSetup")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**TotpSetupResponse**](TotpSetupResponse.md)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="verifyEmail"></a>
# **verifyEmail**
> verifyEmail(verifyEmailRequest)

Verify a user&#39;s email address using a verification token

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AuthApi()
val verifyEmailRequest : VerifyEmailRequest =  // VerifyEmailRequest | 
try {
    apiInstance.verifyEmail(verifyEmailRequest)
} catch (e: ClientException) {
    println("4xx response calling AuthApi#verifyEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AuthApi#verifyEmail")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **verifyEmailRequest** | [**VerifyEmailRequest**](VerifyEmailRequest.md)|  | |

### Return type

null (empty response body)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

