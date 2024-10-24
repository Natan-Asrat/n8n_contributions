# Passed 36 Tests
![unit](https://github.com/user-attachments/assets/5acaa5fb-60af-481e-aa50-737191380b7e)

## Added Fields for Deck
**Color** field in **Create** and **Update** Board operations
**Archived** field in **Update** Board operation only
Renamed **boardName** value sent as **"name"** in request body to **"title"**

### Create Board changes in UI
- Before

![before_createBoard](https://github.com/user-attachments/assets/106fbe5e-e8a5-46da-911c-d17f3337ea18)

- After

![after_createBoard](https://github.com/user-attachments/assets/4396043b-fb50-4f06-a4a0-9de06c9f4262)


### Update Board changes in UI
- Before

![before_updateBoard](https://github.com/user-attachments/assets/35dd073d-042f-4133-b9f2-d9706df395c8)

- After

![after_updateBoard](https://github.com/user-attachments/assets/e49d8d59-51a9-4696-bff9-da9afbce69b3)


## Justification
[Link to docs where request body for **Create** and **Update** operations on Board are specified](https://deck.readthedocs.io/en/latest/API/)

### Create Board Justification (on the right)
![createBoard](https://github.com/user-attachments/assets/96a71be1-1f54-4019-ba38-01f6c31ade13)

### Update Board Justification (on the right)
![updateBoard](https://github.com/user-attachments/assets/8ce062bb-69b3-4c9d-b3eb-b0597b912af6)

## Added Note Fields
**Category** and **Title** Fields along with the **Content** Field in **Create Note** Operation.

- Before

![before_createNote](https://github.com/user-attachments/assets/1a7905e0-e5a7-4b8a-b36c-c26665fc0d44)

- After

![after_createNote](https://github.com/user-attachments/assets/0d16d0e2-f516-46ed-92e2-db3d4cae29d6)


## Added Get Note Operation

- Before

![before_notesList](https://github.com/user-attachments/assets/ed4bd080-b599-47f5-93f8-a25aa0b4d601)

- After 

![after_notesList](https://github.com/user-attachments/assets/3830dbc4-316b-4c25-af38-c3487f98a202)

## Justification
[Link to a NotesService used in Next Cloud that demonstrates how the api should be called](https://github.com/nextcloud/notes/blob/main/src/NotesService.js#L32)
![createNote](https://github.com/user-attachments/assets/cdf771e5-9b18-4434-9ee7-cdbe365de596)


## Added Table Operations
- **Create Column**
- **Get Columns**
- **Get a Column**
- **Update Column**
- **Delete Column**

![added_column_operations](https://github.com/user-attachments/assets/821e76cb-504a-4933-876c-9cf3468e02a7)

- **Create Row**
- **Get Rows**
- **Get a Row**
- **Update Row**
- **Delete Row**

![added_row_operations](https://github.com/user-attachments/assets/3ae48ceb-94d5-45a2-9964-4328659b72a0)


## Added Table Fields
### Create Column Fields

![after_createColumn_first](https://github.com/user-attachments/assets/e2980dc6-d3ba-4cb9-903c-74384f2ea2b3)

#### Number type

![after_createColumn_type_number_1](https://github.com/user-attachments/assets/3cf54d00-0d84-4cf3-b366-6f88a9505388)
![after_createColumn_type_number_2](https://github.com/user-attachments/assets/1bc5bd55-4c58-4716-a7b5-f3e4ca318fa7)

#### Text type

![after_createColumn_type_text](https://github.com/user-attachments/assets/9735a388-13d2-431d-8c13-4819c50e34ac)

#### Selection type

![after_createColumn_type_selection](https://github.com/user-attachments/assets/72e6302b-4fe5-4284-925c-01b00bf29bf6)

#### Datetime type

![after_createColumn_type_datetime](https://github.com/user-attachments/assets/44294570-c8cf-4ade-9683-37acc7ad4d36)

#### User group type

![after_createColumn_type_usergroup_1](https://github.com/user-attachments/assets/b7d9a7d6-af52-4f48-b706-790fb6d43890)
![after_createColumn_type_usergroup_2](https://github.com/user-attachments/assets/73ed2200-549e-4840-8a9a-8440df62f12c)

#### Boolean type

![after_createColumn_type_boolean](https://github.com/user-attachments/assets/db36b0c9-6378-46d8-8057-57ca8255c315)


### Update Column

![after_updateColumn](https://github.com/user-attachments/assets/1733ea10-d992-496a-b2a9-cc8baecd7afe)

### Get a Column

![after_getColumn](https://github.com/user-attachments/assets/6a7a9772-0806-45cd-be34-9b607cebfde0)

### Delete a Column

![after_deleteColumn](https://github.com/user-attachments/assets/e271ff5f-521a-4606-954c-239c7368e8fc)


### Create Row Fields

![after_createRow](https://github.com/user-attachments/assets/f49476c0-d97f-48e4-a7f1-f73cc39f4c08)

### Update Row Fields

![after_updateRow](https://github.com/user-attachments/assets/57fa11cd-01a0-4584-b57a-bfec800b3559)

### Get Rows Fields

![after_getRows](https://github.com/user-attachments/assets/b7825590-c96c-450a-b8a9-3c013f80e0dc)

### Get a Row Fields

![after_getRow](https://github.com/user-attachments/assets/92c98891-ba17-4a62-aede-b43242f576c9)

### Delete Row Fields

![after_deleteRow](https://github.com/user-attachments/assets/8bbf028c-8a0b-4c41-a99d-ed948df637c5)

## Reference for Fields
- [NextCloud Table App Swagger Docs](https://petstore.swagger.io/?url=https://raw.githubusercontent.com/nextcloud/tables/main/openapi.json#/)
- [Definition of types property for Create and Update Columns](https://github.com/nextcloud/tables/blob/main/lib/Service/ImportService.php#L452)

## Tables url change
- /1/ instead of /v1/

## Justification for url change
- [NextCloud Table App Swagger Docs](https://petstore.swagger.io/?url=https://raw.githubusercontent.com/nextcloud/tables/main/openapi.json#/)
- [Use case])(https://help.nextcloud.com/t/using-the-tables-api-partial-success-and-1-problem/172370)

## Added Talk Operations
- **Get Messages**
- **Get Message Context**
- **Update Message**
- **Delete Message**
- **Mark Read**
- **Mark Unread**
- **Get a single conversation**
- **Update conversation**

![after_opsList](https://github.com/user-attachments/assets/a6c60cf1-01ae-447b-a11e-28fe9b868d81)

### Get Messages

![after_getMessages](https://github.com/user-attachments/assets/8965611e-9228-4c22-ae81-527e1d3f75cb)

#### Get Message Context

![after_getMessageContext](https://github.com/user-attachments/assets/e74301d7-4b27-47c3-9073-a847f0a3bceb)

#### Update Message

![after_updateMessage](https://github.com/user-attachments/assets/e005e6f8-ad55-4389-9509-4173f68422f7)

#### Delete Message

![after_deleteMessage](https://github.com/user-attachments/assets/462050d5-cdbe-4c96-a4b1-21ad6cb36bc4)

#### Mark Read

![after_markRead](https://github.com/user-attachments/assets/5ea534f9-4071-43db-8775-b46bda6986f3)

#### Mark Unread

![after_markunread](https://github.com/user-attachments/assets/d992803d-0221-4fb8-b7ff-1da3802f541b)

#### Get a single conversation

![after_getAconversation](https://github.com/user-attachments/assets/58df2bee-5738-4177-a086-65a6f7e6deb0)

### Update conversation

![after_updateConv](https://github.com/user-attachments/assets/8423f0f3-e2cb-4e51-940f-1947cf46f00f)

## API Docs for Conversation
[Conversation Docs](https://nextcloud-talk.readthedocs.io/en/latest/conversation/)
[Messages Docs](https://nextcloud-talk.readthedocs.io/en/latest/chat/)
