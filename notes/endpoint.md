USER
|  Method  |                  Endpoint                    |         Description        |
|----------|----------------------------------------------|----------------------------|
|  GET     |  /api/v1/users/{id}/urls                     |  view list of URL          |
|  GET     |  /api/v1/users/{id}/urls/{url_id}/analytics  |  view url analytics        |
|  POST    |  /api/v1/users/{id}/urls                     |  create new URL            |
|  PATCH   |  /api/v1/users/{id}/urls/{url_id}            |  edit existing URL         |
|  DELETE  |  /api/v1/users/{id}/urls/{url_id}            |  delete existing URL       |
|  PATCH   |  /api/v1/users/{id}                          |  edit account details      |
|  DELETE  |  /api/v1/users/{id}                          |  delete account            |
|  GET     |  /api/v1/email/verify/{id}/{hash}            |  verify account via email  |


ADMIN
|  Method  |                  Endpoint                    |            Description           |
|----------|----------------------------------------------|----------------------------------|
|  GET     |  /api/v1/admin                               |  view system wide analytics      |
|  GET     |  /api/v1/admin/users                         |  view all users                  |
|  GET     |  /api/v1/admin/urls                          |  view all URLs across all users  |
|  PATCH   |  /api/v1/admin/urls/{id}                     |  modify URL details              |
|  DELETE  |  /api/v1/admin/urls/{id}                     |  delete any URL                  |
|  PATCH   |  /api/v1/admin/users/{id}/ban                |  suspend/ban users               |
|  GET     |  /api/v1/admin/log                           |  view audit logs                 |
|  PATCH   |  /api/v1/admin/users/{id}                    |  modify user's data              |
|  DELETE  |  /api/v1/admin/users/{id}                    |  delete user's data              |


AUTH

-> User
|  Method  |                  Endpoint                    |       Description      |
|----------|----------------------------------------------|------------------------|
|  POST    |  /api/v1/register                            |  register account      |
|  POST    |  /api/v1/login                               |  login                 |
|  POST    |  /api/v1/logout                              |  logout                |

-> Admin
|  Method  |                  Endpoint                    |       Description      |
|----------|----------------------------------------------|------------------------|
|  POST    |  /api/v1/admin/login                         |  login                 |
|  POST    |  /api/v1/admin/logout                        |  logout                |


REDIRECT URL | GET | /{slug} <-- 302
|  Method  |                  Endpoint                    |             Description           |
|----------|----------------------------------------------|-----------------------------------|
|  GET     |  /{slug}                                     |  redirect short URL [return 302]  |
