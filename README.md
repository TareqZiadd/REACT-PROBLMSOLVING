# REACT-PROBLMSOLVING
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
