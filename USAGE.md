<!-- Start SDK Example Usage [usage] -->
```typescript
import { MailEngine } from "mailengine";

const mailEngine = new MailEngine({
    bearerAuth: "<YOUR_BEARER_TOKEN_HERE>",
});

async function run() {
    const result = await mailEngine.postSendEmail({
        recipientEmail: "john.doe@example.com",
        recipientName: "John Doe",
        senderEmail: "noreply@example.com",
        senderName: "No Reply",
        emailSubject: "Important Information",
        emailContent: "This is a test email content.",
    });

    // Handle the result
    console.log(result);
}

run();

```
<!-- End SDK Example Usage [usage] -->