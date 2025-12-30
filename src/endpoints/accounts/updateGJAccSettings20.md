# `/accounts/updateGJAccSettings20.php`

Updates a user's account settings.

## Parameters

| Parameter   | Description                                                                                             | Required |
|-------------|---------------------------------------------------------------------------------------------------------|----------|
| `accountID` | The accountID of the user whose account is being updated                                                | Yes      |
| `gjp2`      | The GJP2                                                                                                | Yes      |
| `secret`    | Wmfv3899gc9                                                                                             | Yes      |
| `cS`        | Who the user allows to view their comments: 0 for anyone, 1 for just friends, and 2 for only themselves | No       |
| `frS`       | Who the user allows friend requests from: 0 for anyone, and 1 for no one                                | No       |
| `mS`        | Who the user allows messages from: 0 for anyone, 1 for just friends, and 2 for no one                   | No       |
| `twitch`    | The user's twitch username                                                                              | No       |
| `twitter`   | The user's twitter handle                                                                               | No       |
| `yt`        | The end of the link to the user's youtube channel, after the `/channel/`.                               | No       |

## Response

`1` if the required parameters are passed, regardless of anything is being updated, `-1` otherwise.
