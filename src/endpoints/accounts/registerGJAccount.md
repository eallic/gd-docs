# `/accounts/registerGJAccount.php`

Registers an account.

## Parameters

| Parameter  | Description                           | Required |
|------------|---------------------------------------|----------|
| `email`    | The email of the account to create    | Yes      |
| `password` | The password of the account to create | Yes      |
| `secret`   | Wmfv3899gc9                           | Yes      |
| `userName` | The username of the account to create | Yes      |

## Response

`1` if successful.

## Errors

| Error Code | Meaning                               |
|------------|---------------------------------------|
| -1         | Generic Error                         |
| -2         | Username taken                        |
| -3         | Email taken                           |
| -4         | Username is longer than 20 characters |
| -5         | Invalid Password                      |
| -6         | Invalid Email                         |
| -8         | Password to short                     |
| -9         | Username to short                     |
