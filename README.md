# OrderMenu

This app is built to learn state management in Phoenix LiveView.

## Primary Files and Folders

* **Main LiveView module**:  
  `lib/order_menu_web/live/order_menu_live.ex`

* **Hook**:  
  `assets/js/hooks/order_menu_hook.js`

* **Data source (JSON format)**:  
  `priv/static/data.json`

* **UI design**:  
  `about-project/design`
  
## Start Phoenix server to see the UI and more:

  * Run `mix deps.get` to install dependencies (only for the first time)
  * Run `mix phx.server` or inside IEx with `iex -S mix phx.server`
  * Go to [`localhost:4000`](http://localhost:4000) from your browser.

## What I use + Document recommendations
  * Web Design: [`Frontend Mentor`](https://www.frontendmentor.io/challenges/product-list-with-cart-5MmqLVAp_d)
  * Web Framework: [`Phoenix LiveView`](https://hexdocs.pm/phoenix_live_view/Phoenix.LiveView.html)
  * Language: [`Elixir`](https://hexdocs.pm/elixir/Kernel.html#content)
  * CSS Library: [`TailwindCSS`](https://tailwindcss.com/)

## Notes
  * State Naming: `snake_case` only. E.g. ->  is_clicked
  * ERB tag (Embedded Ruby tag): `<%= ... %>`
  ### handle_event/3
   * We can have as many handle_event/3 functions as you need, there's no strict limit.
     ⚠️ **BUT** put specific ones first and catch-all patterns last to avoid conflicts—Elixir matches from top to bottom.
   * Each one should match on a different event name (or different pattern).
   * Elixir uses pattern matching, so when a LiveView receives an event, it tries each handle_event/3 function until it finds one that matches the event name.

## LEARN MORE
  * Examples: [`Phoenix LiveView Examples`](https://a4word.com/articles/liveview-examples)
  * Article: [`Import, Alias, Require, and Use in Elixir`](https://gabriel.perales.me/blog/import-alias-require-and-use)
