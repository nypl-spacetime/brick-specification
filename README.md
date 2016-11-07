
# Tasks specification for brick-by-brick

Data specification for [brick-by-brick](https://github.com/nypl-spacetime/brick-by-brick) tasks and submissions. This document does not specify *how* to interact with a brick-by-brick API, but only *what* data a client application is expected to receive and send. For brick-by-brick's API specification, see https://github.com/nypl-spacetime/brick-by-brick#api.

## Read item for task

```js
{
  "id": "itemId",
  "data": {
    // item task data, valid for this task
    // See below
  },
  "organization": {
    "id": "organizationId"
  },
  "collection": {
    "id": "collectionId"
  }
}
```

Note: `organitionId` together with`itemId` uniquely identify an item.

## Write task submission for item

```js
{
  "id": "itemId",
  "organization": {
    "id": "organizationId"
  },
  "task": {
    "id": "taskId"
  }
  "data": {
    // item submission data, valid for this task
    // See below
  }
}

## Read task submission for item

```js
{
  "step": "default",
  "data": {
    // item submission data, valid for this task
    // See below
  },
  "dateCreated": "2016-11-04T20:26:33.869Z",
  "dateModified": "2016-11-04T20:26:33.869Z",
  "task": {
    "id": "taskId"
  }
  "collection": {
    "id": "collectionId"
  },
  "organization": {
    "id": "organizationId"
  },
  "item": {
    "id": "itemId"
  }
}
```

# Tasks

## `geotag-photo`

Item task data:

Submission data:

## `geotag-text`

Item task data:

Submission data:

## `select-toponym`

Item task data:

Submission data:
