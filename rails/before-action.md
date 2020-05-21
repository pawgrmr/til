###Before Action

Before filter provided by rails to call a method before a particular Rails Controller action.
Goes at the top of a Rails controller. By default they apply to *every* action in a controller
but it is possible to restrict them to certain actions by passing the `only:` hash like in the example below.

Usage:

`before_action :method, only: [:edit, :update]`
The method called `method` in this case is to be called before the `edit` and `update` controller actions.
The `method` will be located in the `private` section of the controller.
