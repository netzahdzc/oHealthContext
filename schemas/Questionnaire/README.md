# Questionnaire

## Description

Set of questions regarding the physical test performance.

## Data Model

A JSON Schema corresponding to this data model can be found [here](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/Questionnaire/questionnaire-1.x.json).

+ `id` : Unique identifier. 
    + Mandatory.

+ `type` : Entity type. It must be equal to `Questionnaire`.
    + Mandatory.

+ `refUser` : Reference to the actual User sheltered by an independent service.
    + Attribute type: `string`.
    + Mandatory.

+ `question` : Word or set of words that represent a particular question related to health.
    + Attribute type: [question](https://github.com/netzahdzc/oHealth-Context/blob/master/schemas/dataType/question-1.x.json).
    + Mandatory.  

+ `dateModified` : Last entity's update timestamp.
    + Attribute type: [DateTime](https://schema.org/DateTime).
    + Mandatory. 

## Examples of use

```
{
  "id": "ffffffffff9cbbf4465f0ef30033c587-questionnaire-7118",
  "type": "Questionnaire",
  "test": {
    "value": "ffffffffff9cbbf4465f0ef30033c587-test-71108",
    "type": "test-identification"
  },
  "refUser": "http://207.249.127.162:1234/users/1",
  "question": {
    "value": "true",
    "type": "answer-to-question"
  },
  "dateModified": {
    "value": "2017-01-18T20:45:42.697Z-0800",
    "type": "DateTime"
  }
}
```

    
## Use it with a real service

T.B.D.

## Open Issues

T.B.A.