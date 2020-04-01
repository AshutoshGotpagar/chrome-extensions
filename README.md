--Extension Types--

1. Browser Action

- Stay in toolbar
- Accessible at all times

2. Page Action

- Stay in tool bar but grey-ed out
- Accessible only on certain pages

3. Neither BA or PA

- Run in background

--Manifest File--

- Special file that has information about the extension
- It is in JSON format
- Mandatory details that must be included are

1. Manifest version
2. Name of the Extension
3. Veriosn of the Extension

--Chrome Storage--

- The chrome.storage API is used to store, retrieve, and track changes to user data.
- To use this we must declare "storage" permission in the extension manifest.

--Options Page--

- Aside from the popup page we can have another page called 'options page' which can be viewed when right clicking on the icon of the extension.

--Background Page v/s Event Page--

- 2 types of pages - background and event
- Background page runs at all times
- Event page runs only when required
- background pages consume resources even when not required
- Stick to event pages

--Content Scripts--

- Run in the context of the web page
- Can change DOM, font color, hyperlinks and structure DOM,
- Limitation - Can't use all chrome Api's
- To fully utilise Context scripts we need to exchange messages between context scripts, backgroud scripts and popup scripts
