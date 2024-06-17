# Salesforce Objects List for Pentesting

This repository contains a comprehensive list of Salesforce API objects, intended for use in pentesting Salesforce applications. The list can be utilized for fuzzing objects and identifying potential vulnerabilities.

## Contents

- `salesforce_objects.txt`: A text file containing the full list of Salesforce API objects.

## Usage

This list can be used in pentesting activities to automate the process of fuzzing Salesforce objects and identifying potential security issues.

### Example

Here’s an example of how you might read the `salesforce_objects.txt` file in Python:

Burp Steps

```

    1. Send any POST with an Aura endpoint to Repeater

    2. Replace the “message” parameter in your request with the below options.

    3. Send it to Intruder

    4. Choose *** in the params (objectApiName, entityNameOrId) as the position in Intruder

    5. Let “payload type” remain as Simple List

    6. Upload the objects.txt file or paste the objects list in “payload options” and run it for all objects whenever possible
```

Note - You can fuzz them both as a guest user and as different authenticated users to understand permissions
[Salesforce API objects](https://developer.salesforce.com/docs/atlas.en-us.object_reference.meta/object_reference/sforce_api_objects_list.htm)
[Pentesting Salesforce Apps](https://infosecwriteups.com/in-simple-words-pen-testing-salesforce-saas-application-part-2-fuzz-exploit-eefae11ba5ae)
