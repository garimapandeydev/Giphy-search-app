# Giphy Search App

This is a simple Vue.js application that allows users to search for GIFs using the Giphy API. The app displays GIFs based on user input and allows the user to copy the URL of any GIF to their clipboard.

## Features

- Search GIFs: Users can type in a search term, and the app will fetch relevant GIFs from the Giphy API.
- **GIF Preview**: Display GIFs as background images in a grid layout.
- **Copy GIF URL**: Users can easily copy the original GIF URL to the clipboard.
- **Responsive Design**: The app is responsive and adjusts to different screen sizes.

## Project Structure

### Components

1. **Gif.vue**: Displays an individual GIF with a background image and a button to copy the GIF URL.
2. **GifList.vue**: Displays a list of GIFs passed down as props.
3. **SearchInput.vue**: Contains the input field where users type in their search queries. It triggers a search when the user types and sends the search results to the parent component.

### App.vue

This is the main component that brings together the search input and GIF list components. It listens for the search results and updates the displayed GIFs.

### Styles

The application uses simple scoped CSS to style the components. It employs Flexbox for layout and responsive design.

## Setup

### Requirements

- Node.js (v12 or later)
- Vue CLI

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/giphy-search-app.git
   cd giphy-search-app
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm run serve
   ```

4. Open your browser and navigate to `http://localhost:8080` to see the app in action.

## API

This app uses the Giphy API to fetch GIFs. You can sign up for your own Giphy API key at [https://developers.giphy.com/](https://developers.giphy.com/) if needed.

### API Endpoint

- **Search GIFs**: `https://api.giphy.com/v1/gifs/search?api_key=YOUR_API_KEY&q={searchTerm}&limit=9`


