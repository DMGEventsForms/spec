# Fields

## Defaults

These are assumed by default with all the fields:

1. Fields that are not shown in the form will not have their field names submitted as part of the request payload

## Requirements

Below are the fields that make up the form templates. The field names are **bolded** in the title.

### Email Address (**emailAddress**)

This is used as a unique identifier for the person who submitted the form.

- Field: Text
- Validated if it looks like an e-mail

### First Name (**firstName**)

The person's first name.

- Field: Text

### Last Name (**lastName**)

The person's last name.

- Field: Text

### 1st Line Street Address (**address1**)

The first line of address. Used for sending event brochures and other promotional artefacts.

- Field: Text

### 2nd Line Street Address (**address2**)

The second line of address. Used for sending event brochures and other promotional artefacts.

- Field: Text

### Postal Code (**postCode**)

The short code to their address.

- Field: Text

### Country (**country**)

The country they're in.

- Field: Single Select
- Be able to select one from a list of countries

### City (**city**)

The city of the country they're in.

- Field: Single Select
- Disable field until the [Country](#country-country) field is filled in
- Be able to select one from a list of cities based on country

### Company Name (**companyName**)

The company they represent, if applicable.

- Field: Text

### Job Title (**jobTitle**)

Their job title in the company, if applicable e.g. Software Engineer, Director.

- Field: Text

### Job Function (**jobFunction**)

Their department in the company.

- Field: Text

### Mobile Number (**mobileNumber**)

e.g. `+447763971285`

- Field: Text
- Displays the area code's country once entered
- Errors on an invalid mobile phone number

### Telephone Number (**telephoneNumber**)

e.g. `03451720088`

- Field: Text
- Displays the area code's country once entered
- Errors on an invalid telephone number

### Fax Number (**faxNumber**)

e.g. `555-123-4567`

- Field: Text
- Displays the area code's country once entered
- Errors on an invalid fax number

### Industry (**industry**)

The company's nature of business category e.g. `Oil & Gas`.

- Field: Single Select
- Be able to select one from a list of industries
- Should have varying combinations of industries in different lists based on the brand

### Event Interests (**interests**)

The list of services or products in the event that the person is interested in.

- Field: Multi Select
- Be able to select one or more from a list of interests
- Should have varying combinations of interests in different lists based on the brand

### Type of Interest (**interestType**)

Will indicate what role they'll want to be doing in the event

- Field: Single Select
- Should have varying combinations of interest types in different lists based on the brand
- Example options are:

```json
[
  { "value": "sponsor", "label": "Sponsoring the event" },
  { "value": "attendee", "label": "Attending the event" },
  { "value": "speaker", "label": "Speaking at the event" }
]
```

### Level of Interest (**interestLevel**)

The degree of motivation that they want to participate in the event.

- Field: Single Select
- Should have varying combinations of interest levels in different lists based on the brand
- Example options are:

```json
[
  { "value": "research", "label": "I would like more information" },
  { "value": "review", "label": "I would like to get a quote/cost" },
  { "value": "ready", "label": "I would like to book/register" }
]
```

### Influence (**influence**)

The type of influence the person will have in the case they'll want to purchase something in the event.

- Field: Radio Group
- The options are fixed:

```json
[
  { "value": "influencer", "label": "Influencer" },
  { "value": "purchaser", "label": "Purchaser/Buyer" },
  { "value": "executive", "label": "Influencer" },
  { "value": "endUser", "label": "End User" },
  { "value": "noPower", "label": "No Influencing Power" }
]
```

### Level of Influence (**influenceLevel**)

The level of monetary influence the person will have in case they'll want to purchase something in the event.

- Field: Radio Group
- The options are fixed:

```json
[
  { "value": "low", "label": "Up to $100,000" },
  { "value": "med", "label": "Up to $500,000" },
  { "value": "high", "label": "Above $500,000" }
]
```

### SACAP Number (**sacapNumber**)

A phone number for SACAP (South African Council for the Architectural Profession).

- Field: Text

### ECSA Number (**ecsaNumber**)

A phone number for ECSA (Engineering Council of South Africa)

- Field: Text
