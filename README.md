# JsonBox for Node

## Usage

```javascript
const { JsonBox } = require('jsonbox-node');

async function() {
    const jbn = new JsonBox();

    // Create a record
    await jbn.create({
        name: "Test",
        age: 42
    }, BOX_ID);

    // Read records
    await jbn.read(BOX_ID);

    // Update a record
    await jbn.update({ age: 43 }, BOX_ID, recordId);

    // Delete a record
    await jbn.delete(BOX_ID, recordId)

    // Delete a record set
    await jbn.deleteMany(BOX_ID, recordIds);
}
```
