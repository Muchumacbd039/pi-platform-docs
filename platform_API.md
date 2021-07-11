# Platform API

The platform API allows you to read and write data to the Pi Servers related with your app deployed on the
Pi App Platform, and your app's users.

## Overview

### Base path:api.minepi.com/v2

The latest version of the Platform API is available at `api.minepi.com/v2`.

> **Note about API versioning:**
>
> The platform API is currently in v2.
> As much as possible, we will not make any breaking changes to a version of an API, and only release breaking changes as
> new major versions. However, we might make breaking changes to an existing version without notice, if those are
> necessary (e.g security or privacy fixes).

### Authorization

#### Server API Key authorization

For various reasons, some API calls must be made from your backend / server app.
Those endpoints can be accessed using the following Authorization header:

```
Authorization: Key <k4bbcg68yryws74rq8o3woelf2qdfjhmnhm26jhx9nvrsctzvjhbelfhmv4pm4qfp>
```

> **Warning: Server API keys are for servers only**
>
> Your Server API Key **must** be kept on your server, and must not be sent to clients (do not use it in your
> client javascript code).
> In the future, your server API key might enable sensitive operations on your app itself that your users should
> not be allowed to perform. Letting users access your server API key is a **serious security breach**.

