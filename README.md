# Discovery Meeting Agenda Pages

Customizable pre-call briefing pages for Loophire sales prospects, hosted on Netlify.

## Structure

```
├── templates/
│   └── base-template.html    # Master template with placeholders
├── prospects/
│   └── [prospect-name].html  # Generated prospect-specific pages
```

## Template Variables

| Variable | Description |
|----------|-------------|
| `{{PROSPECT_NAME}}` | Prospect's first name |
| `{{CALL_DATE_TIME}}` | Meeting date/time |
| `{{PRIORITY_1}}` | First pain point/priority |
| `{{PRIORITY_2}}` | Second pain point/priority |
| `{{PRIORITY_3}}` | Third pain point/priority |
| `{{RESCHEDULE_LINK}}` | Calendly or booking link |

## Workflow

1. Have discovery conversation with prospect
2. Customize template based on call transcript
3. Save to `prospects/[name].html`
4. Deploy to Netlify
5. Share personalized URL with prospect

## Deployment

Connected to Netlify for automatic deployments on push to `main`.
