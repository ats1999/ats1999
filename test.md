# <span style="color:#b20101">Is it possible to connect the react component to the redux store without export default?</span>

<span style="color:#2b0000">Many times we want to connect to the redux store without exporting it from the `.js | .jsx | .ts | .tsx`  file. The reason we want to do it is we can not make a separate file for each small component. Suppose we have 1000s of small components and 100s of main `React` component. We can make 100s of files for the main component but we can not make another 1000s of file for the small components.</span>

### <span style="color:#ff00dc">TOC</span>

1. <span style="color:#4970bd">What is React </span>`Small Introduction`
2. <span style="color:#4970bd">What is redux </span>`Small Introduction`
3. <span style="color:#4970bd">What is reducer</span>
4. <span style="color:#4970bd">What is HOC</span>
5. <span style="color:#4970bd">What is the connect method of </span>`Redux`
6. <span style="color:#ff0000">Main problem.</span>

<br>
<span style="color:#c343a5">1\. What is React?</span>
<span style="color:#000000">A JavaScript library for building user interfaces. </span>
<span style="color:#080076">Feature</span>

* Declarative
* Component-based
* Learn once write anywhere.

[Learn more about it from https://reactjs.org/](https://reactjs.org/)

<span style="color:#c343a5">2\. What is Redux?</span>
<span style="color:#010106">A Predictable State Container for JS Apps.</span>
<span style="color:#010106">Feature</span>

* Predictable
* Centralized
* Debuggable
* Flexible

[Learn more about it from https://redux.js.org/](https://redux.js.org/)

<span style="color:#d200cb">3\. What is reducer in Redux?</span>
`Reducer` specify how the application state changes in response to the action sent to the store. The action only states that what happened in the application but it does not specify how the application state changes.

<span style="color:  #d200cb;;">4\. What is HOC?</span>
The <i>**HOC**</i>  stands for <b>*higher-order components.*</b>

<span style="color:#d200cb">5\. What is the connect method if `Redux`?</span>
The Task of the connect method  `React-Reduc` is to connect with the `Redux-store`. <span style="color:  #1c1e21;;">It does not modify the component class passed to it; instead, it returns a new, connected component class that wraps the component you passed in.</span>
