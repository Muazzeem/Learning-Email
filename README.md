**E-mail Template**


Create New SES Template:

1. crate a json file.

```json
{
  "Template": {
    "TemplateName": "Template-name",
    "SubjectPart": "Email-subject",
    "HtmlPart": "Html content"
  }
}
```
2. Create SES Email templates 
```shell
    $ aws ses create-template --cli-input-json file://json-file-path
```

3. Update Email templates
```shell
    $ aws ses update-template --cli-input-json file://json-file-path
```

Need more information:
1. [Youtube Video](https://www.youtube.com/watch?v=64Ut2HZbyWw)
2. [AWS Doc](https://docs.aws.amazon.com/ses/latest/APIReference/API_Template.html)
3. [Stackoverflow](https://stackoverflow.com/questions/50207457/aws-ses-template-html-part-is-multiple-lines)