# Drum Kit

- Thẻ audio: src là đường dẫn của file âm thanh

    ```html
    <audio data-key="76" src="sounds/tink.wav"></audio>
    ```

    ```jsx
    const audio = document.querySelector(`audio[data-key="${e.keyCode}"]`);

    if(!audio) return;

    audio.currentTime = 0;
    audio.play(); // PLAY THẺ AUDIO 
    ```

- Sự kiện 'keydown'

    ```jsx
    window.addEventListener('keydown', playSound);
    ```

- Sự kiện kết thúc css transition 'transitionend'

    ```jsx
    keys.forEach(key => key.addEventListener('transitionend', removeTransition));
    ```