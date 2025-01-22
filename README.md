# Calendar Event Manager
Written in TypeScript.

### Tools/Technologies/Libraries used

- React (Main UI Library)
- React Draggable
- React Select (UI library)
- Firebase (BaaS)
- User Authentication using Firebase(Google Account)
- Calender API (Date and time API)
- Typescript (A superset language of JS)
- Sass (Stylesheet Lanuage)

## Available Features

- [x] Calendars
- [x] Mini Calendar
- [x] Schedules: Event and Task
- [x] Calendar View Selection: Day, Week, and last 4 days
- [x] Draggable dialog w/ readjustable position
- [X] Time Indicator (fully displayed in the current day column)
- [x] External Holiday Events
- [x] User Settings
- [x] User Authentication with Firebase (Google account)
- [X] Firebase Firestore

### Required configuration for .env Variables

**Client-side Configuration**

1. Create the following env files under /client: `.env` and `.env.development`
2. Define this variable `REACT_APP_HOLIDAY_API_URL` in each file accordingly.

_For example_:

```dotenv
REACT_APP_HOLIDAY_API_URL=https://your-holiday-api-url.com
```

3. Create the following .env variables under /server:

- `API_KEY`: Generate your API key [here](https://console.cloud.google.com/)
- `CALENDAR_ID`: By default, the value should be always `holiday@group.v.calendar.google.com`
- `CALENDAR_REGION (optional)`: If you're unsure about the value to initialize, use the following value: `en.usa`. To find the available options, refer to the list of supported regions on this [file](./client/src/data/localized-holiday-events.txt).

_For example_

```dotenv
API_KEY=your-api-key
CALENDAR_REGION=en.usa
CALENDAR_ID=holiday@group.v.calendar.google.com
```


