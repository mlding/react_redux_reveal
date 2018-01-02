##  events classification

- Native events - when component mount, through addEventListener to bind event is browser's native events, when using native events, must manually using removeEventListener to remove binding when component unmount

- Synthetic events(recommend) - using the way of event delegation add binding to the top layer of component, will destroy binding event automatically when component unmount
