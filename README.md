Sproutcore Notes
================

SC.ArrayController
- `status`, `property`, `this.get('status')`


SC.ObjectController
- `contentBinding`, `various(?)`, `contentBinding: "booksController.selection"`


SC.State
- `enterState`, `function`, `enterState: function() {}`, (Called by SC, Default Empty, Override to use. )
- `exitState`, `function`, `exitState: function() {}`, (Called by SC, Default Empty, Override to use. )
- `gotoState`, `function`, `this.gotoState(state, context)`
  - String `state`, Name of the state
  - Mixed `context`, Context
- `initializeSubstate`, `various`, `initializeSubstate: [String|SC.State]`, (Default Empty, Override to use. )


SC.Statechart
- `trace`, `property`, `trace: [YES|NO]`
