# React Hooks

## features
```
1.use React without Class.(Hooks dont't work inside classes)
2.使用{function}useState,this function returns a pair:the current state value and a function that let you updates it.
3.可在一个component中定义多个state
4.use {function} useEffect,this function runs after every render.And it can optional returns a function that React performs when the component unmounts.
```

## grammar
```javascript
import {useState} from 'react';

function Example(props){
    const[stateName,setStateName]=useState(initialState);
    const[todos,setTodos]=useState([{text:'work'}]);

    setEffect(()=>{
        ChatAPI.subscribeToFriendStatus(props.friend.id,handleFunction);
        return ChatAPI.unsbuscribeToFriendStatus(props.friend.id,handleFucntion);
    })

    setEffect(()=>{document.title=<div>{todos}</div>},[todos]);//only run if props todos are diferrent from the previous value
    function handleFunction(){}
    return(
        <div>
            <p>show state's value:{stateName}</p>
            <label>setState:</label><button onClick={()=>setStateName(state)}>Click me</button>
        </div>
    )
}
```
