# hypermedian-manifesto
> "Make it Hypermedian!"

The Web Developement (_Sites_ & especially _Applications_) in both industry & the academy need to return to their rich roots of Hypermedia in web applications & websites, while still preserving the hard-fought-for gains in user-interactivity that so-called "Modern" (transl.: "Fashionable") Web Apps (_esp. Single-Page Application Frameworks_), thus creating a category that is both old & new: "_**Hypermedian**_" (_also called by some "Hypermedia Driven Apps," or HDAs_).

## Table of Contents:

## Why?  Why Hypermedian?
> Because our Web Applications are getting too complex and slow, by fighting the medium they target (the browser, primarily), because the browsers do not implement Hypermedia in a fully, truly Hypermedian way, and thus Developers usually ignore the Intrinsically Hypermedia-oriented natures of browsers, to the detriment of User Experience, of the inordinately high number of developers needed to develop a Web Application, & of Developer's own productivity!  Inexorably, the high number of developers and large number and arbitrary division of labor into teams runs up against [Conway's Law](https://martinfowler.com/bliki/ConwaysLaw.html), which many developers, architects, managers, and executives have either forgotten or never known in the first place.  Conway's Law is:
> "Any organization that designs a system (defined broadly) will produce a design whose structure is a copy of the organization's communication structure."

It is best explained in great detail & depth [in this video](https://www.youtube.com/watch?v=5IUj1EZwpJY).

Hypermedian Apps reduce the amount of complexity in building Web Applications (_& even Native Applications as well!_) by recognizing what Hypermedia Systems were supposed to be, using their native functionality where it exists, and augmenting a browser's unimplemnted Hypermedia functionality (_That SHOULD Just Be There_) until such time as the browsers implement it natively (at which point the augmentation scripting would be deprecated/eventually-removed in favor of using the built-in Hypermdia functionality.

Hypermedia Systems are not well-understood (Here's a helpful book called ["Hypermedia Systems"](https://hypermedia.systems), which you can purchase a copy or read for FREE online, by Carson Gross, creator of HTMX, even if HTMX is problematic from a truly, fully Hypermedian perspective), so let's dive into defining Hypermedian terms to better understand when we talk about them.


## Definitions:

### What is "Hypermedian?"
> "Adhering to the pseudo-cultus of Web Applications/Sites driven by, & oriented to, Hypermedia, that is, HyperText & hypermedia controls, which have behaviors following strict hypermedia protocols and their specifications, & filled with content, structure, scripting, & security features, driven by the User & the User-Agent, with the single source of truth residing in one or more data stores, with the Hypermedia Server acting as the conduit to that single source of truth."  Hypermedian Apps adhere to the strict, correct definitions of being Hypermedia-driven, with HATEOAS & ReST as helpful concepts to guide one to designing or building, or both, a Hypermedia System.

## OK, so What do you mean by "Hypermedia" now?
> "Hypermedia" is the provenance/use of a combination of built-in interfaces & well-defined protocols, having & centered around the following concomittant behaviors & properties:

- _**HyperText**_ (_Text that triggers a HyperText Protocol action, according to some HyperText Protocol Specification, e.g., leading to other pages or sections, etc._)
- _**HyperText Controls**_ (_Elements that trigger HyperText Protocol actions, according to some HyperText Protocol Specification, e.g., submitting a form button sending data to the server and navigating to a new page, etc._)
- A _**HyperText Protocol**_: a medium of navigation and a Control Plane for such navigation, driven by HyperText, HyperText Controls, or both, as well as:
  - _Zero or more **Users**_
  - _One or more **User-Agents**_
  - _Typically One **Hypermedia Server**, but there could be more than one_ (e.g., in _Peer-to-Peer_ communications like _**WebRTC**_, the User-Agent (_usually a Browser_) acts as both User-Agent _**AND**_ Hypermedia Server!)
- A _**HyperText Protocol Specification**_ (spec), for communication/sharing (_e.g., via an HTTP 1.1 Spec-based protocol_):
  - (_...future standardized protocol specs..._)
  - HTTP 3
  - HTTP 2
  - HTTP 1.1
  - HTTPS 3
  - HTTPS 2
  - HTTPS 1.1
  - PHTTP 3
  - PHTTP 2
  - PHTTP 1.1
  - (_...with maybe more bespoke specs to come in the future...?_)
- _**Content**_ (_i.e., "elements"_)
  - Typographical Graphics (_i.e., hypermedia elements containing "Text", and subject to intrinsic _)
  - Display elements (_e.g., "**div**," "**span**," or "**dialog**" elements, to name only a few..._ there are too many to list here)
  - Raster Graphics (_e.g., "image" elements, or certain icons_: smaller than an equivalent Vector Graphic, but can become "lossy" with certain resizings...)
  - Vector Graphics (_e.g., "svg" elements, i.e., "Scalable Vector Graphics", or certain icons_: resizable without loss, but larger than an equivalent Raster Graphic.)
  - Audio elements
  - Video elements
  - ...
  - Custom elements (i.e., Server-defined elements not in the HTML spec, interpreted by the User-Agent as if a built-in element, with definable special behavior per custom-element. There are two types:
    - "**Autonomous**" (_those whose definitions extend the `HTMLElement`_)
    - "**Customized**" (_those whose definitions extend a given existing element (other than `HTMLElement`, e.g., `HTMLAnchorElement`) to decorate it with new behavior or behaviors!_)
- _**Structure**_ (_i.e., "markup" + (implicitly) "styling"... in reality, markup & styling are actually coupled, usually tightly, but sometimes in a simple, elegant loose fashion..._)
  - HTML5 Markup (_+ Styling_)
  - PHTML5 Markup (_+ Styling_)
- _**Styling**_ (as defined by):
  - Style element rules (_e.g., "CSS," or "Cascading Style Sheets", but there could theoretically be other formats_)
  - Element attributes (_i.e., An HTML element's certain attribute's content, for example_):
    - An HTML element's direct definition of its CSS styles via an element's "style" attribute's (well-formed) content (_so-called "**Inline Styles"**_)
    - An HTML element's direct redefinition of custom CSS Variables via an element's "style" attribute's content (_as yet to be named... "Inline Restyles?"..._) [aside: BE BRAVE & TRY TO FIND IT A GOOD NAME: WE NEED ONE FOR THIS LITTLE-USED TECHNIQUE!]
    - An HTML element's indirect CSS styling based off of more concrete status of its `class` attribute (_so-called "**Class Styles**"_)
    - An HTML element's indirect CSS styling based off of more abstract status of its `class` attribute (_so-called "**Utility Styles**"_)
    - An HTML element's implicit CSS Styling based off of direct global rules (_like `element` CSS selector-based rules_)
    - An HTML element's implicit CSS Styling based off of indirect global rules (_like `*` CSS selector-based rules_)
    - An HTML element's explicit CSS Styling based off of direct global rules (_i.e., styling off of `id` attributes (e.g., `#id_name`), as there can only be one HTML element in a given document with a certain `id`!)
- _**Scripts**_:
  - Typically "_**ECMAScript**_" (_commonly referred to as "**JavaScript**"_).  This language was both designed & implemented in approximately only 10 days, to allow web developers to add interactivity to the browser.
  - Sometimes "_**WebAssembly**_" (_also often called "**Wasm**", as it is shorter to both write and say_).  This language comes from a transpilation from another language, to be run by the User-Agent via ECMAScript.  It is more efficient both to parse & to run, but it has limitations: it is sandboxed from the Browser's _**DOM**_ ("_Document Object Model_," which is the bridge between the native code of the User-Agent, and the scripting code of the Server, or sometimes (_malicious?_) User (_/Attacker?_)), may have limitations on its ability to share memory, and must be written in a language (typically a Low-Level language, which not everybody can do even in the first place, and far fewer can do it even somewhat well _(cf. "Data-Oriented Design")_)... but there are exceptions, and theoretically it IS possible to handwrite WebAssembly...)
- _**Security**_
  - _...**shh...** we can't let the Black Hats know our secrets or they'll get us..._

> The Combination of Data Store and Hypermedia-driven Web Server, together with the browser's implementation, & augmentation by script, makes possible the construction of a Hypermedian Web App.  The combination of the set or sets of developers working on that Web Application allow or deny the Web Application's being truly Hypermedian, first by the organizational & communication structures by which they are architected, second by Conway's Law and the limits it imposes on large team structures, & third by the (often fashionable & flashy new whizbang) tools & techniques with which those developers build the application/system.

This Manifesto is a call to reduce the complexity of building Web Applications, without losing the interactivity we have come to expect from the use of Modern, non-Hypermedian tools & techniques, & without resorting to the Modern (_read: "Fasionable"_) Way Of Doing Things.  Majority opinion does not make Reality, and Truth is the mind's conformity to Reality: by observing Reality, rethinking our preconceptions, conforming our minds to Reality, and forming new conceptions upon which to act, we can build things with far less complexity, far fewer develoeprs, which together allow for far greater feats to accomplish!


#### Categories that fall under "Hypermedian":
- Static HTML websites
- Static PHTML websites
- HTML-driven web applications/sites
- PHTML-driven web applications/sites

#### Categories that do NOT fall under the umbrella of "Hypermedian":
- JSON-driven web applications
- XML-driven applications


### What is "CRUD?"
> "_**CRUD**_" stands for "**Create**", "**Read**", "**Update**", & "**Delete**."

It refers to the mapping of HTTP Methods grossly to Database actions, even when there is an impedence mismatch between how the Database Management System stores data at rest, and how the Web Server Stores the data in motion.  This generates significant complexity for the sake of oversimplifying HTTP methods.  In a CRUD system, "Create" would be implemented by HTTP `POST`, "Read" by HTTP `GET`, "Update" by HTTP `PUT` (_&, **occasionally**, HTTP `PATCH`), & "Delete" by HTTP `DELETE`.

> `TODO`: finish this section?

### What is "HATEOAS?" 
> "**HATEOAS**" stands for: "_**H**ypermedia **A**s **T**he **E**ngine **O**f **A**pplication **S**tate_".

It refers to the Server's unique role of bearing the single source of truth, and the User-Agent/Browser/Native-App's state being a mere reflection of that Server state.  All modifications to state are triggered by the User or the User-Agent/Browser/Native-App by means of Hypermedia, and not by making data-exchange calls.  

> `TODO`: finish this section?

...

### What is REST (or ReST)?
> "_**ReST**_" stands for: "_**Re**presentational **S**tate **T**ransfer_".

`TODO`: finish this section!

...

### What is PHTML?
> "_**PHTML**_" stands for: "_**P**ost-**HTML**_," or "_**P**ost **H**yper**T**ext**M**arkup**L**anguage_".

`TODO`: finish this section!


### What is HTM$?
> "_**HTM$**_" stands for: "_**H**yper**T**ext**M**edia**$**treaming/morphing_".

`TODO`: finish this section!

