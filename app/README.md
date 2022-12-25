# Support Ticket System Backend <!-- omit in toc -->

## Table of Contents <!-- omit in toc -->

- [Route Structure](#route-structure)
- [Ticket Structure](#ticket-structure)
  - [Example](#example)

## Route Structure

| Route                     | Status | Comment                   |
| :-----------------------: | :----: | :------------------------ |
| `/`                       | 🚧     | Homepage                  |
| `/login`                  | ❌     | Log in page               |
| `/signup`                 | ❌     | Sign up page              |
| `/signup/forgot_password` | ❌     | Forgot Password page      |
| `/dashboard`              | ❌     | Dashboard page            |
| `/tickets`                | ❌     | Support tickets list page |
| `/about`                  | 🚧     | About page                |
| `/settings`               | ❌     | Settings page             |

## Ticket Structure

| Field               | Comment                                                                  |
| :------------------ | :----------------------------------------------------------------------: |
| Id                  | Ticket hash ID                                                           |
| Name                | Name of the ticket issuer                                                |
| Date                | Date in which the ticket was issued                                      |
| First Status Change | First time the ticket status has changed                                 |
| Last Update         | Date in which the ticket was last updated                                |
| Priority            | How urgent the ticket is (1 to 5, higher number means higher priority)   |
| Status              | Current ticket status: [`In queue` \| `In work` \| `Rejected` \| `Done`] |

### Example

```json
{
    "id": 6538,
    "name": "John",
    "date": "10.12.2013 14:52",
    "first_status_change": "11.12.2013 18:22",
    "last_update": "13.12.2013 09:35",
    "priority": 3,
    "status": "in queue"
}
```
