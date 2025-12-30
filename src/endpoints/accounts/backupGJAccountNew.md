# `/accounts/backupGJAccountNew.php`

Saves account data.

**Note:** This page is on the account server. You can find the domain name by sending a request to /database/getAccountURL.php (currently http://www.robtopgames.org).

## Parameters

| Parameter       | Description                                                                               | Required |
|-----------------|-------------------------------------------------------------------------------------------|----------|
| `binaryVersion` | 42                                                                                        | Yes      |
| `gameVersion`   | 22                                                                                        | Yes      |
| `password`      | The password of the account to be added                                                   | Yes      |
| `saveData`      | A gzip-compressed CCGameManager.dat, a semicolon, and a gzip-compressed CCLocalLevels.dat | Yes      |
| `secret`        | Wmfv3899gc9                                                                               | Yes      |
| `userName`      | The username of the account to be added                                                   | Yes      |
| `gdw`           | 0                                                                                         | No       |

## Response

`1` if data was saved, `-1` if not.
