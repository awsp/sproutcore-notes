Sproutcore Notes
================

SC.ArrayController
- `status`, `property`, `this.get('status')`
- `content`, `property`, `this.get('content')`, (Important property, holds all data)
- `selection`, `property`, (Important property, current selected object. )
- `arrangedObjects`, `property`, (Important property, similar to content, but in the processed way such as orderBy)


SC.ObjectController
- `contentBinding`, `various(?)`, `contentBinding: "MyApp.booksController.selection"`


SC.State
- `enterState`, `function`, `enterState: function() {}`, (Called by SC, Default Empty, Override to use. )
- `exitState`, `function`, `exitState: function() {}`, (Called by SC, Default Empty, Override to use. )
- `gotoState`, `function`, `this.gotoState(state, context)`
  - String `state`, Name of the state
  - Mixed `context`, Context
- `initializeSubstate`, `various`, `initializeSubstate: [String|SC.State]`, (Default Empty, Override to use. )


SC.Statechart
- `trace`, `property`, `trace: [YES|NO]`, (Print trace messages in console. )



------------


### Utilities
- `static_url`, `SC Helper`, (Non-JS function, SC-specified helper, Used to load static images. )
  - `background: static_url('images/message.png') 0 0 no-repeat;`
  - Location is based on current location. Namely, `resources` folder


### Deployment
```
$ sproutcore build app_name [--mode=my_mode]
```

- Destination at `tmp/build/static/myapp/en/{HASH}/`
- Use `--mode` to specific which mode/configuration it will use. 
