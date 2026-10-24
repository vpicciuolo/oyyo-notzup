<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Personal Booking Pages and Meeting Links

Every NotzUp user can have a personal public page for meetings and appointments. Share one link and let guests choose from the times you make available, shown in the guest's own time zone. Guests do not need a NotzUp account to request or confirm an available time.

Booking pages are an account service. They do not upload recordings, transcripts or local AI results, and they do not start a recording when a meeting begins.

## Create your personal booking page

1. Sign in to the NotzUp web app.
2. Open **Calendar** or **Bookings**.
3. Create an event type, such as a 30-minute consultation or a 15-minute introduction.
4. Set the public title, description and meeting duration.
5. Add the days and hours when guests may book.
6. Set a minimum notice period so a guest cannot book too close to the start time.
7. Add a buffer before or after each meeting when you need preparation or travel time.
8. Review the time zone shown for your account.
9. Preview the public page and copy your personal booking link.

Your public page shows only booking information intended for guests. It does not expose your private calendar, recordings, files, local searches or other NotzUp content.

## Share a booking link

Send the personal page link by email, message, website or another channel you control. A guest opens the page, sees available times in their own time zone, enters the requested booking details and confirms an available slot.

Do not publish a private management link. The public booking link is for guests; a private management link is for the named booking participant to review, reschedule or cancel that specific appointment.

## Avoid double bookings

NotzUp checks current availability when the guest confirms a time. Availability can reflect bookings already stored in NotzUp and, when a supported external calendar is connected and working, eligible busy times returned under the permissions you approved.

An external calendar affects availability only after you authorize the connector and its configuration succeeds. Signing in with Google or Microsoft does not automatically give NotzUp calendar access.

## Confirmation, rescheduling and cancellation

After confirmation, the booking can include:

- the agreed date and time in the participant's time zone;
- the meeting title and approved guest instructions;
- an `.ics` calendar file where supported;
- a private link for the participant to manage that booking;
- configured in-app, email or device notifications.

Use the private management link or the authenticated Bookings area to reschedule or cancel. A provider invitation or email notification is sent only when that delivery channel has been configured and enabled.

## Booking limits and plans

Confirmed booking limits depend on the account plan and the current UTC billing month. A booking-page limit is separate from recording duration, local processing and device enrollment. Changing a meeting time should not silently create a second appointment; always review the booking record after a reschedule.

## Privacy and consent

- A booking page collects only the information requested for scheduling.
- Local recordings, transcripts, scans and searches are not attached to a booking unless the user deliberately shares something separately.
- Connecting an external calendar uses the provider's official consent screen and the scopes shown there.
- Disconnect an unused provider from NotzUp and from the provider's own security settings.
- Obtain participant consent before recording a meeting. A confirmed appointment is not recording consent.

## Troubleshooting

### A guest sees no available times

Check the event type's active days, hours, time zone, minimum notice, buffers and date range. Then check existing bookings and any connected calendar that can mark time busy.

### The displayed time looks wrong

Verify the account time zone and ask the guest to confirm the time zone detected by the booking page. Daylight-saving rules can change the local clock even when the underlying appointment remains correct.

### A calendar event was not created

The NotzUp booking may still be valid. Check the connector status, provider permission scopes and configuration. Download or import the `.ics` file when available.

### A guest cannot change the appointment

Use the private management link from the confirmation. If the link has expired or is unavailable, manage the booking from the authenticated NotzUp account and send the guest the updated confirmation.

## Related guides

- [Complete User Guide](USER_GUIDE.md)
- [Local-First Privacy and Data Control](LOCAL_FIRST_PRIVACY.md)
- [FAQ](FAQ.md)

