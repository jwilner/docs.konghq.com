---
title: deck ping
---

The ping command can be used to verify if decK
can connect to Kong's Admin API.

```
deck ping [flags]
```

### Options

```
  -h, --help               help for ping
  -w, --workspace string   Ping configuration with a specific Workspace (Kong Enterprise only).
                           Useful when RBAC permissions are scoped to a Workspace.
```

### Options inherited from parent commands

```
      --analytics                      Share anonymized data to help improve decK. (default true)
      --ca-cert string                 Custom CA certificate to use to verify Kong's Admin TLS certificate.
                                       This value can also be set using DECK_CA_CERT environment variable.
      --config string                  Config file (default is $HOME/.deck.yaml).
      --headers strings                HTTP headers (key:value) to inject in all requests to Kong's Admin API.
                                       This flag can be specified multiple times to inject multiple headers.
      --kong-addr string               HTTP address of Kong's Admin API.
                                       This value can also be set using the environment variable DECK_KONG_ADDR
                                        environment variable. (default "http://localhost:8001")
      --konnect-addr string            Address of the Konnect endpoint. (default "https://konnect.konghq.com")
      --konnect-email string           Email address associated with your Konnect account.
      --konnect-password string        Password associated with your Konnect account, this takes precedence over --konnect-password-file flag.
      --konnect-password-file string   File containing the password to your Konnect account.
      --no-color                       Disable colorized output
      --skip-workspace-crud            Skip API calls related to Workspaces (Kong Enterprise only).
      --timeout int                    Set a request timeout for the client to connect with Kong (in seconds). (default 10)
      --tls-server-name string         Name to use to verify the hostname in Kong's Admin TLS certificate.
                                       This value can also be set using DECK_TLS_SERVER_NAME environment variable.
      --tls-skip-verify                Disable verification of Kong's Admin TLS certificate.
                                       This value can also be set using DECK_TLS_SKIP_VERIFY environment variable.
      --verbose int                    Enable verbose logging levels
                                       Setting this value to 2 outputs all HTTP requests/responses
                                       between decK and Kong.
```

### See also

* [deck](/deck/{{page.kong_version}}/reference/deck)	 - Administer your Kong clusters declaratively
