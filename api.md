The base api can be found at `https://testapi.photodino.de/`. 

`BASE_URL for =  https://testapi.photodino.de/`

## Events
GET

|Action |URL |Parameters |Response |
|--|--|--|--|
|get all events |`BASE_URL/events/` |`None`|Array with diciontaries for each event
|Get specific city |`BASE_URL/events/<event_id>` |`None` |Dictonary array of event details
Filter by  name|`BASE_URL/events/` | `{"name": "str"}` |List of all events matching name or not found message

POST

|Action |URL |Parameters |Response
|--|--|--|--|
|Create new event |`BASE_URL/events/` |[event object](#event_object) |created event json object

PUT

|Action |URL |Parameters|Response
|--|--|--|--|
|Update existing event |`BASE_URL/events/<event_id>/` | [event object](#event_object) |updated event json||object

DELETE

|Action |URL |Parameters |Response
|--|--|--|--|
|Delete event |`BASE_URL/events/<event_id>/` |`None` |`None` or `Not found`

### <a name=event_object|></a> `event_object`
|Attribute |Type |Example |Default 
|-- |-- |-- |--
|id |`int` |23 |auto
|events |`array` |[1, 3 ,4 ,5] |auto
|name |`str` |Birthday |`None`
|description |`str` | This event is a birthday party for a young boy |auto
|event_date |`date` | 22.1.2022 |auto
