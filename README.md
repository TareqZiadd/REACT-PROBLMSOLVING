# REACT-PROBLMSOLVING


#https://momentjs.com/
rerer اكتب ساعة باستخدام رياكت باللغة الانجليزية داخل كومبونينت


import React, { useState } from 'react';

Function Time () {
  const [currentTime, setCurrentTime] = useState(new Date().toLocaleTimeString());

  function updateTime () {
    setCurrentTime(new Date().toLocaleTimeString());
  }
  setInterval(updateTime, 1000);

  return (
    <div>
      <div>
      <h1>{currentTime}</h1>
      </div>
    </div>
  );
}

export default Time;


d اعمل نفس الساعة ولكن باللغة العربية

import React, { useState } from 'react';
import "../index.css"
import moment from 'moment';
import 'moment/locale/ar';  
const Time = () => {
  
  const [currentTime, setCurrentTime] = useState(moment().format('LTS'));

  function updateTime () {
    setCurrentTime(moment().format('LTS'));
  }
  setInterval(updateTime, 1000);

  return (
    <div>
      <div>
      <h1>{currentTime}</h1>
      </div>
    </div>
  );
}

export default Time;

---------------------------------------------------------------------------------------------
