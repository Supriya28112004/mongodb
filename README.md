<pre>
 use todo
switched to db todo   

 
db.todos.insertMany([
  {
    title: "Buy groceries",
    description: "Milk, Bread, Eggs, Fruits",
    status: "pending",
    dueDate: new Date("2025-06-01"),
    priority: "high"
  },

  
  {
    title: "Read a book",
    description: "Read 'Atomic Habits'",
    status: "completed",
    dueDate: new Date("2025-05-25"),
    priority: "low"
  },


  
  {
    title: "Pay electricity bill",
    description: "Pay before due date to avoid penalty",
    status: "pending",
    dueDate: new Date("2025-06-05"),
    priority: "medium"
  },

  
  {
    title: "Finish project report",
    description: "Finalize and submit to guide",
    status: "in-progress",
    dueDate: new Date("2025-05-30"),
    priority: "high"
  }
])


{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6836e39cf59ddb70e4428073'),
    '1': ObjectId('6836e39cf59ddb70e4428074'),
    '2': ObjectId('6836e39cf59ddb70e4428075'),
    '3': ObjectId('6836e39cf59ddb70e4428076')
  }
  
}
 
db.todos.insertMany([
  {
    title: "Buy groceries",
    description: "Milk, Bread, Eggs, Fruits",
    status: "pendin",
    dueDate: new Date("2025-06-01"),
    priority: "high"
  },


  
  {
    title: "Read a book",
    description: "Read 'Atomic Habits'",
    status: "completed",
    dueDate: new Date("2025-05-25"),
    priority: "low"
  },

  
  {
    title: "Pay electricity bill",
    description: "Pay before due date to avoid penalty",
    status: "pending",
    dueDate: new Date("2025-06-05"),
    priority: "medium"
  },

  
  {
    title: "Finish project report",
    description: "Finalize and submit to guide",
    status: "in-progress",
    dueDate: new Date("2025-05-30"),
    priority: "high"
  }

  
])


{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6836e585f59ddb70e4428077'),
    '1': ObjectId('6836e585f59ddb70e4428078'),
    '2': ObjectId('6836e585f59ddb70e4428079'),
    '3': ObjectId('6836e585f59ddb70e442807a')
  }


  
}
db.todos.updateMany(
  { status: "completed" },
  { $set: { status: true } }
);
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 3,
  modifiedCount: 3,
  upsertedCount: 0
}



db.todos.insertMany([
  {
    title: "Call the plumber",
    description: "Fix the leaking kitchen sink",
    status: false,
    dueDate: new Date("2025-06-02"),
    priority: "medium"
  },

  
  {
    title: "Schedule dentist appointment",
    description: "Annual dental check-up",
    status: false,
    dueDate: new Date("2025-06-10"),
    priority: "low"
  },


  
  {
    title: "Workout session",
    description: "1 hour at the gym",
    status: false,
    dueDate: new Date("2025-05-29"),
    priority: "high"
  },
  {
    title: "Plan weekend trip",
    description: "Decide location and book hotel",
    status: false,
    dueDate: new Date("2025-06-03"),
    priority: "medium"
  },
  {
    title: "Clean the garage",
    description: "Organize tools and boxes",
    status: false,
    dueDate: new Date("2025-06-01"),
    priority: "low"
  },
  {
    title: "Submit tax documents",
    description: "Upload to government portal",
    status: true,
    dueDate: new Date("2025-05-27"),
    priority: "high"
  }
])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6836e601f59ddb70e442807b'),
    '1': ObjectId('6836e601f59ddb70e442807c'),
    '2': ObjectId('6836e601f59ddb70e442807d'),
    '3': ObjectId('6836e601f59ddb70e442807e'),
    '4': ObjectId('6836e601f59ddb70e442807f'),
    '5': ObjectId('6836e601f59ddb70e4428080')
  }
}
db.todos.find({})
{
  _id: ObjectId('6836e2759678cca1a0c276fd'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: 'pending',
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e2759678cca1a0c276fe'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e2759678cca1a0c276ff'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: 'pending',
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e2759678cca1a0c27700'),
  title: 'Finish project report',
  description: 'Finalize and submit to manager',
  status: 'in-progress',
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e39cf59ddb70e4428073'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: 'pending',
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e39cf59ddb70e4428074'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e39cf59ddb70e4428075'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: 'pending',
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e39cf59ddb70e4428076'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: 'in-progress',
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e585f59ddb70e4428077'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: 'pendin',
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e585f59ddb70e4428078'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e585f59ddb70e4428079'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: 'pending',
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e585f59ddb70e442807a'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: 'in-progress',
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e601f59ddb70e442807b'),
  title: 'Call the plumber',
  description: 'Fix the leaking kitchen sink',
  status: false,
  dueDate: 2025-06-02T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e601f59ddb70e442807c'),
  title: 'Schedule dentist appointment',
  description: 'Annual dental check-up',
  status: false,
  dueDate: 2025-06-10T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e601f59ddb70e442807d'),
  title: 'Workout session',
  description: '1 hour at the gym',
  status: false,
  dueDate: 2025-05-29T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e601f59ddb70e442807e'),
  title: 'Plan weekend trip',
  description: 'Decide location and book hotel',
  status: false,
  dueDate: 2025-06-03T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e601f59ddb70e442807f'),
  title: 'Clean the garage',
  description: 'Organize tools and boxes',
  status: false,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e601f59ddb70e4428080'),
  title: 'Submit tax documents',
  description: 'Upload to government portal',
  status: true,
  dueDate: 2025-05-27T00:00:00.000Z,
  priority: 'high'
}
db.todos.find().pretty()
{
  _id: ObjectId('6836e2759678cca1a0c276fd'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: 'pending',
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e2759678cca1a0c276fe'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e2759678cca1a0c276ff'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: 'pending',
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e2759678cca1a0c27700'),
  title: 'Finish project report',
  description: 'Finalize and submit to manager',
  status: 'in-progress',
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e39cf59ddb70e4428073'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: 'pending',
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e39cf59ddb70e4428074'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e39cf59ddb70e4428075'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: 'pending',
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e39cf59ddb70e4428076'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: 'in-progress',
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e585f59ddb70e4428077'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: 'pendin',
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e585f59ddb70e4428078'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e585f59ddb70e4428079'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: 'pending',
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e585f59ddb70e442807a'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: 'in-progress',
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e601f59ddb70e442807b'),
  title: 'Call the plumber',
  description: 'Fix the leaking kitchen sink',
  status: false,
  dueDate: 2025-06-02T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e601f59ddb70e442807c'),
  title: 'Schedule dentist appointment',
  description: 'Annual dental check-up',
  status: false,
  dueDate: 2025-06-10T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e601f59ddb70e442807d'),
  title: 'Workout session',
  description: '1 hour at the gym',
  status: false,
  dueDate: 2025-05-29T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e601f59ddb70e442807e'),
  title: 'Plan weekend trip',
  description: 'Decide location and book hotel',
  status: false,
  dueDate: 2025-06-03T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e601f59ddb70e442807f'),
  title: 'Clean the garage',
  description: 'Organize tools and boxes',
  status: false,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e601f59ddb70e4428080'),
  title: 'Submit tax documents',
  description: 'Upload to government portal',
  status: true,
  dueDate: 2025-05-27T00:00:00.000Z,
  priority: 'high'
}
db.todos.find({status:false})
{
  _id: ObjectId('6836e601f59ddb70e442807b'),
  title: 'Call the plumber',
  description: 'Fix the leaking kitchen sink',
  status: false,
  dueDate: 2025-06-02T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e601f59ddb70e442807c'),
  title: 'Schedule dentist appointment',
  description: 'Annual dental check-up',
  status: false,
  dueDate: 2025-06-10T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e601f59ddb70e442807d'),
  title: 'Workout session',
  description: '1 hour at the gym',
  status: false,
  dueDate: 2025-05-29T00:00:00.000Z,
  priority: 'high'
}
{
  _id: ObjectId('6836e601f59ddb70e442807e'),
  title: 'Plan weekend trip',
  description: 'Decide location and book hotel',
  status: false,
  dueDate: 2025-06-03T00:00:00.000Z,
  priority: 'medium'
}
{
  _id: ObjectId('6836e601f59ddb70e442807f'),
  title: 'Clean the garage',
  description: 'Organize tools and boxes',
  status: false,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'low'
}
db.todos.find({status:true})
{
  _id: ObjectId('6836e2759678cca1a0c276fe'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e39cf59ddb70e4428074'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e585f59ddb70e4428078'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low'
}
{
  _id: ObjectId('6836e601f59ddb70e4428080'),
  title: 'Submit tax documents',
  description: 'Upload to government portal',
  status: true,
  dueDate: 2025-05-27T00:00:00.000Z,
  priority: 'high'
}
db.todos.insertMany([
  {
    title: "Call the plumber",
    description: "Fix the leaking kitchen sink",
    status: false,
    dueDate: new Date("2025-06-02"),
    priority: "medium"
  },
  {
    title: "Schedule dentist appointment",
    description: "Annual dental check-up",
    status: false,
    dueDate: new Date("2025-06-10"),
    priority: "low"
  },
  {
    title: "Workout session",
    description: "1 hour at the gym",
    status: false,
    dueDate: new Date("2025-05-29"),
    priority: "high"
  },
  {
    title: "Plan weekend trip",
    description: "Decide location and book hotel",
    status: false,
    dueDate: new Date("2025-06-03"),
    priority: "medium"
  },
  {
    title: "Clean the garage",
    description: "Organize tools and boxes",
    status: false,
    dueDate: new Date("2025-06-01"),
    priority: "low"
  },
  {
    title: "Submit tax documents",
    description: "Upload to government portal",
    status: true,
    dueDate: new Date("2025-05-27"),
    priority: "high"
  }
])
{
  acknowledged: true,
  insertedIds: {
    '0': ObjectId('6836e855f59ddb70e4428081'),
    '1': ObjectId('6836e855f59ddb70e4428082'),
    '2': ObjectId('6836e855f59ddb70e4428083'),
    '3': ObjectId('6836e855f59ddb70e4428084'),
    '4': ObjectId('6836e855f59ddb70e4428085'),
    '5': ObjectId('6836e855f59ddb70e4428086')
  }
}
db.todos.updateMany(
  { status: { $exists: false } },
  { $set: { status: false } }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todos.updateMany(
  { status: { $exists: true} },
  { $set: { status: false } }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 24,
  modifiedCount: 14,
  upsertedCount: 0
}
db.todos.updateMany(
  { status: { $exists: true} },
  { $set: { status: false } }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 24,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todos.insertOne({
  title: "New Task",
  description: "This task has no status set explicitly",
  status: false,  // manually setting default
  dueDate: new Date(),
  priority: "medium"
})
{
  acknowledged: true,
  insertedId: ObjectId('6836e9a7f59ddb70e4428087')
}
db.todos.updateMany(
  { status: { $exists: true} },
  { $set: { status: false } }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 25,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todos.updateOne(
  { _id: ObjectId("6656372d9abf0f173ca3fc2a") },
  { $set: { status: true } }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todos.updateMany(
  { status: false },
  {
    $set: {
      status: true,
      updatedAt: new Date()
    }
  }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 25,
  modifiedCount: 25,
  upsertedCount: 0
}
db.todos.updateMany(
  { status: false },
  {
    $set: {
      status: true,
      updatedAt: new Date()
    }
  }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todos.updateMany(
  { status: false },
  {
    $set: {
      status: true,
      updatedAt: new Date()
      createdAt: new Date() }
  }
)
SyntaxError: Unexpected token, expected "," (7:6)

[0m [90m  5 |[39m       status[33m:[39m [36mtrue[39m[33m,[39m
 [90m  6 |[39m       updatedAt[33m:[39m [36mnew[39m [33mDate[39m()
[31m[1m>[22m[39m[90m  7 |[39m       createdAt[33m:[39m [36mnew[39m [33mDate[39m() }
 [90m    |[39m       [31m[1m^[22m[39m
 [90m  8 |[39m   }
 [90m  9 |[39m )
 [90m 10 |[39m[0m
db.todos.updateMany(
  { },
  {
    $set: {
      createdAt:new Date()
      updatedAt: new Date()
    }
  }
)
SyntaxError: Unexpected token, expected "," (6:6)

[0m [90m 4 |[39m     $set[33m:[39m {
 [90m 5 |[39m       createdAt[33m:[39m[36mnew[39m [33mDate[39m()
[31m[1m>[22m[39m[90m 6 |[39m       updatedAt[33m:[39m [36mnew[39m [33mDate[39m()
 [90m   |[39m       [31m[1m^[22m[39m
 [90m 7 |[39m     }
 [90m 8 |[39m   }
 [90m 9 |[39m )[0m
db.todos.updateMany(
  { status: false },
  {
    $set: {
      status: true,
      updatedAt: new Date()
    }
  }
)

{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todos.updateMany(
  {},
  {
    $set: {
      createdAt: new Date(),
      updatedAt: new Date()
    }
  }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 25,
  modifiedCount: 25,
  upsertedCount: 0
}
db.todos.find({})
{
  _id: ObjectId('6836e2759678cca1a0c276fd'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e2759678cca1a0c276fe'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e2759678cca1a0c276ff'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: true,
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e2759678cca1a0c27700'),
  title: 'Finish project report',
  description: 'Finalize and submit to manager',
  status: true,
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428073'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428074'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428075'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: true,
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428076'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: true,
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e4428077'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e4428078'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e4428079'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: true,
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e442807a'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: true,
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807b'),
  title: 'Call the plumber',
  description: 'Fix the leaking kitchen sink',
  status: true,
  dueDate: 2025-06-02T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807c'),
  title: 'Schedule dentist appointment',
  description: 'Annual dental check-up',
  status: true,
  dueDate: 2025-06-10T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807d'),
  title: 'Workout session',
  description: '1 hour at the gym',
  status: true,
  dueDate: 2025-05-29T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807e'),
  title: 'Plan weekend trip',
  description: 'Decide location and book hotel',
  status: true,
  dueDate: 2025-06-03T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807f'),
  title: 'Clean the garage',
  description: 'Organize tools and boxes',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e4428080'),
  title: 'Submit tax documents',
  description: 'Upload to government portal',
  status: true,
  dueDate: 2025-05-27T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e855f59ddb70e4428081'),
  title: 'Call the plumber',
  description: 'Fix the leaking kitchen sink',
  status: true,
  dueDate: 2025-06-02T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e855f59ddb70e4428082'),
  title: 'Schedule dentist appointment',
  description: 'Annual dental check-up',
  status: true,
  dueDate: 2025-06-10T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
Type "it" for more
db.todos.updateMany(
  { priority: { $exists: false } },
  { $set: { priority: "medium" } }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todos.find({})
{
  _id: ObjectId('6836e2759678cca1a0c276fd'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e2759678cca1a0c276fe'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e2759678cca1a0c276ff'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: true,
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e2759678cca1a0c27700'),
  title: 'Finish project report',
  description: 'Finalize and submit to manager',
  status: true,
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428073'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428074'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428075'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: true,
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428076'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: true,
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e4428077'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e4428078'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e4428079'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: true,
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e442807a'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: true,
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807b'),
  title: 'Call the plumber',
  description: 'Fix the leaking kitchen sink',
  status: true,
  dueDate: 2025-06-02T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807c'),
  title: 'Schedule dentist appointment',
  description: 'Annual dental check-up',
  status: true,
  dueDate: 2025-06-10T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807d'),
  title: 'Workout session',
  description: '1 hour at the gym',
  status: true,
  dueDate: 2025-05-29T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807e'),
  title: 'Plan weekend trip',
  description: 'Decide location and book hotel',
  status: true,
  dueDate: 2025-06-03T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807f'),
  title: 'Clean the garage',
  description: 'Organize tools and boxes',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e4428080'),
  title: 'Submit tax documents',
  description: 'Upload to government portal',
  status: true,
  dueDate: 2025-05-27T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e855f59ddb70e4428081'),
  title: 'Call the plumber',
  description: 'Fix the leaking kitchen sink',
  status: true,
  dueDate: 2025-06-02T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e855f59ddb70e4428082'),
  title: 'Schedule dentist appointment',
  description: 'Annual dental check-up',
  status: true,
  dueDate: 2025-06-10T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:04:05.330Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
Type "it" for more
db.runCommand({
  collMod: "todos",
  validator: {
    $jsonSchema: {
      bsonType: "object",
      required: ["priority"],
      properties: {
        priority: {
          enum: ["low", "medium", "high"],
          description: "Must be low, medium, or high"
        }
      }
    }
  },
  validationLevel: "strict",
  validationAction: "error"
})
MongoServerError[AtlasError]: user is not allowed to do action [collMod] on [todo.todos]
db.todos.updateMany(
  {},
  {
    $set: {
      updatedAt: new Date()
    }
  }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 25,
  modifiedCount: 25,
  upsertedCount: 0
}
db.todos.updateOne(
  { _id: ObjectId("6836e855f59ddb70e4428082") },
  {
    $set: {
      status: true,
      updatedAt: new Date()
    }
  }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 1,
  modifiedCount: 1,
  upsertedCount: 0
}
db.todos.countDocuments
[Function: countDocuments] AsyncFunction {
  apiVersions: [ 1, Infinity ],
  serverVersions: [ '4.0.3', '999.999.999' ],
  returnsPromise: true,
  topologies: [ 'ReplSet', 'Sharded', 'LoadBalanced', 'Standalone' ],
  returnType: { type: 'unknown', attributes: {} },
  deprecated: false,
  platforms: [ 'Compass', 'Browser', 'CLI' ],
  isDirectShellCommand: false,
  acceptsRawInput: false,
  shellCommandCompleter: undefined,
  help: [Function (anonymous)] Help
}
db.todos.countDocuments({})
25
db.todos.updateMany(
  { dueDate: { $exists: false } },
  { $set: { dueDate: new Date("2025-05-29") } }
)
{
  acknowledged: true,
  insertedId: null,
  matchedCount: 0,
  modifiedCount: 0,
  upsertedCount: 0
}
db.todos.find({})
{
  _id: ObjectId('6836e2759678cca1a0c276fd'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e2759678cca1a0c276fe'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e2759678cca1a0c276ff'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: true,
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e2759678cca1a0c27700'),
  title: 'Finish project report',
  description: 'Finalize and submit to manager',
  status: true,
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428073'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428074'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428075'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: true,
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e39cf59ddb70e4428076'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: true,
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e4428077'),
  title: 'Buy groceries',
  description: 'Milk, Bread, Eggs, Fruits',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e4428078'),
  title: 'Read a book',
  description: "Read 'Atomic Habits'",
  status: true,
  dueDate: 2025-05-25T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e4428079'),
  title: 'Pay electricity bill',
  description: 'Pay before due date to avoid penalty',
  status: true,
  dueDate: 2025-06-05T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e585f59ddb70e442807a'),
  title: 'Finish project report',
  description: 'Finalize and submit to guide',
  status: true,
  dueDate: 2025-05-30T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807b'),
  title: 'Call the plumber',
  description: 'Fix the leaking kitchen sink',
  status: true,
  dueDate: 2025-06-02T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807c'),
  title: 'Schedule dentist appointment',
  description: 'Annual dental check-up',
  status: true,
  dueDate: 2025-06-10T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807d'),
  title: 'Workout session',
  description: '1 hour at the gym',
  status: true,
  dueDate: 2025-05-29T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807e'),
  title: 'Plan weekend trip',
  description: 'Decide location and book hotel',
  status: true,
  dueDate: 2025-06-03T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e442807f'),
  title: 'Clean the garage',
  description: 'Organize tools and boxes',
  status: true,
  dueDate: 2025-06-01T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e601f59ddb70e4428080'),
  title: 'Submit tax documents',
  description: 'Upload to government portal',
  status: true,
  dueDate: 2025-05-27T00:00:00.000Z,
  priority: 'high',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e855f59ddb70e4428081'),
  title: 'Call the plumber',
  description: 'Fix the leaking kitchen sink',
  status: true,
  dueDate: 2025-06-02T00:00:00.000Z,
  priority: 'medium',
  updatedAt: 2025-05-28T11:13:14.150Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
{
  _id: ObjectId('6836e855f59ddb70e4428082'),
  title: 'Schedule dentist appointment',
  description: 'Annual dental check-up',
  status: true,
  dueDate: 2025-06-10T00:00:00.000Z,
  priority: 'low',
  updatedAt: 2025-05-28T11:16:38.924Z,
  createdAt: 2025-05-28T11:04:05.330Z
}
Type "it" for more
Atlas atlas-c2ctdz-shard-0 [primary] todo



</pre>
