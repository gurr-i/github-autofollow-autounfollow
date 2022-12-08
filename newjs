// Import the Axios library
const axios = require('axios');

// Your GitHub username and personal access token
const username = 'YOUR_USERNAME';
const token = 'YOUR_PERSONAL_ACCESS_TOKEN';

// Function to follow a user
async function followUser(user) {
  // Make a PUT request to the "following" endpoint to follow the user
  const response = await axios.put(
    `https://api.github.com/user/following/${user}`,
    {},
    {
      auth: {
        username,
        password: token
      }
    }
  );
  console.log(`Successfully followed user ${user}`);
}

// Function to unfollow a user
async function unfollowUser(user) {
  // Make a DELETE request to the "following" endpoint to unfollow the user
  const response = await axios.delete(
    `https://api.github.com/user/following/${user}`,
    {
      auth: {
        username,
        password: token
      }
    }
  );
  console.log(`Successfully unfollowed user ${user}`);
}

// Example usage
followUser('githubuser1');
followUser('githubuser2');
unfollowUser('githubuser3');
