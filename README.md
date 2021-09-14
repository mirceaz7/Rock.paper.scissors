# Rock.paper.scissors
First game in JS

const getUserChoice = userInput => {
  userInput = userInput.toLowerCase();
  if (userInput === 'rock' || userInput === 'paper' || userInput === 'scissors' || userInput === 'bomb'){
    return userInput;
  } 
  }

function getComputerChoice() {
  let outcome = Math.floor(Math.random()*3)
  switch (outcome) {
  case 0 : return 'rock';
  case 1 : return 'paper';
  case 2 : return 'scissors';
  }
  }

function determineWinner(userChoice,computerChoice){
  if (userChoice === computerChoice){
    return('The game is a tie!')
  }
  if(userChoice === 'rock'){
    if(computerChoice ==='schissors'){
      return('You win!')
      } else {return('You lose!')}}
  if(userChoice === 'paper'){
    if(computerChoice === 'rock'){
      return('You win!')
      } else {return('You lose!')}}
  if(userChoice === 'scissors'){
    if(computerChoice === 'paper'){
      return('You win!')
      } else {return('You lose!')}}
  if(userChoice === 'bomb'){
    return 'You win!!!'} // cheat code
  }

  console.log(determineWinner('',''))
