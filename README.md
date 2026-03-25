✅ Step 1 → Fetch Main Record

Gets Representative Service record → base data source.

✅ Step 2 → Fetch Contact Email

Because lookup only gives ID
You must fetch full Contact record.

✅ Step 3 → Fetch Child Company Email

Optional secondary recipient logic.

✅ Step 4 → Fetch Owner Details

Using Users API → because phone is NOT always available in record owner object.

✅ Step 5 → Prepare Dynamic HTML Message

Generic
Reusable
Regulatory neutral
No brand dependency

✅ Step 6 → Prepare Mail Merge Structure

Important keys:

mail_merge_template
from_address
to_address
type = attachment
message
✅ Step 7 → Send via v5 Mail Merge API

Correct endpoint:

/Representative_Service/{id}/actions/send_mail_merge
