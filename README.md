# Blueprints for Offshore Hook

## Purpose

This hook's responsibilities are:

1. Use `sails.modules` to read blueprints from the user's app into `self.middleware`.
2. Bind shadow routes to blueprint actions and controller actions.
3. Listen for `route:typeUnknown` on `sails`, interpret route syntax which should match a blueprint action, and bind the appropriate middleware (this happens when the Router is loaded, after all the hooks.)
