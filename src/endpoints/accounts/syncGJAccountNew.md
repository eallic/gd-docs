# `/accounts/syncGJAccountNew.php`

Loads account data.

**Note:** This page is on the account server. You can find the domain name by sending a request to /database/getAccountURL.php (currently http://www.robtopgames.org).

## Parameters

| Parameter       | Description                    | Required |
|-----------------|--------------------------------|----------|
| `accountID`     | The accountID loading the data | Yes      |
| `gjp2`          | The GJP2                       | Yes      |
| `secret`        | Wmfv3899gc9                    | Yes      |
| `binaryVersion` | 42                             | No       |
| `gameVersion`   | 22                             | No       |
| `gdw`           | 0                              | No       |

## Response

A list of values, separated by semicolons `;`:

- saveData sent when saving (note that this value contains a `;`, so it's effectively 2 values)
- gameVersion sent when saving
- binaryVersion sent when saving
- a list of rated levels separated by commas `,`, in the format `[levelID],[stars]`, compressed with deflate and a random string of *20* characters at the front and back
- a list of map pack objects separated by pipes `|`, with keys 1, 3, 4 and 5, compressed with deflate and a random string of *20* characters at the front and back
