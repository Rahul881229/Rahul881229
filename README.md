- console.log("welcome to spotify");

let songIndex = 0;
let audio1="1.mp3.mp3";
let audioElement = new Audio(audio1);

let masterPlay = document.getElementById('masterPlay');
let myProgressBar = document.getElementById('myprogressbar');  
let playPause = document.getElementById('playpause');  
let play = document.getElementById('play');  
let Pause = document.getElementById('pause');  
let  isPlay = true;
console.log(playPause);

let songs = [
    {songName : "salam -e-isq", filepath: "song/1.mp3", coverpath: "covers/1.jpg.jpeg"},
//     {songName : "salam -e-isq", filepath: "song/1.mp3", coverpath: "covers/1.jpg"},
//     {songName : "salam -e-isq", filepath: "song/1.mp3", coverpath: "covers/1.jpg"},
//     {songName : "salam -e-isq", filepath: "song/1.mp3", coverpath: "covers/1.jpg"},
//     {songName : "salam -e-isq", filepath: "song/1.mp3", coverpath: "covers/1.jpg"},
//     {songName : "salam -e-isq", filepath: "song/1.mp3", coverpath: "covers/1.jpg"},
]

Pause.style.display = "none"

playPause.addEventListener('click', ()=>{
    if(isPlay){
    audioElement.play();
        isPlay=false;
        play.style.display = "none"
        Pause.style.display = "block"


    }
    else{audioElement.pause();
    isPlay=true;
    Pause.style.display = "none"
    play.style.display = "block"
}
})

// 
// handle play/pause click
// masterPlay.addEventListener('click', ()=>{
//     if(audioElement.paused || audioElement.currentTime<=0){
//         audioElement.play();
//     }
// })

// listen to events
myProgressBar.addEventListener('timeupdate',  ()=>{
    console.log('timeupdate');
})
👋 Hi, I’m @Rahul881229
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Rahul881229/Rahul881229 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
