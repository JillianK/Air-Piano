# Air-Piano
Introduction:

  This project is a web app that allows users to play the piano without a keyboard and includes modules for basic instruction. Using the Leap Motion to track the user’s movements, the program plays notes of different pitches and volumes based on the positions of the user’s fingers. The user’s hands and position relative to the notes are be displayed on the user’s computer using Three.js.


Development:

  This web app uses the Leap Motion, the Leap Motion JavaScript API, and Three.js to track the hands of the user and play the pitches of the middle three octaves of the piano based on the user’s hand and finger positions. Each pitch was assigned a rectangular area in the x-z plane referred to as the “pitch plane”. The height of the plane in the y axis was set for optimum user comfort and LeapMotion tracking accuracy and range. The pitch locations are displayed on screen as a set of Three.js BoxGeometry objects resembling a traditional piano keyboard.
  
  The user’s hands are presented on screen in relation to the pitches using Three.js. Using finger location data from the LeapMotion, finger bones are represented by CylinderGeometry objects and joints are portrayed by SphereGeometry objects. When a user’s fingertip breaches the pitch plane in a location assigned to a pitch, the note is played. 
  
  In addition to “Classic Mode” for individual user exploration of the technology, the program includes teaching modules. In “Learning Mode”, users can learn the position of notes in the pitch plane. The program prompts the user with the name of a note for the user to play. Upon successfully playing the prompted note, the user receives a point and the program selects a new pitch for the user to find. For more advance users, “Accompaniment Mode” allows users to play the melody from Hoagy Carmichael and Frank Loesser’s 1938 song, “Heart and Soul” as the program loops the accompaniment part.  
