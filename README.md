# Dify Chat Frontend

A simple and modern chat interface for Dify API, built with React and Tailwind CSS.

## Features

- Clean and responsive UI
- Real-time chat interface
- Easy integration with Dify API
- Loading states and error handling
- Auto-scroll to latest messages

## Setup

1. Clone the repository:
```bash
git clone https://github.com/your-username/dify-chat-frontend.git
cd dify-chat-frontend
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory with your Dify API settings:
```env
REACT_APP_DIFY_API_KEY=your_api_key_here
REACT_APP_DIFY_API_URL=http://your-dify-server:5000/v1
```

4. Start the development server:
```bash
npm start
```

The app will be available at `http://localhost:3000`.

## Environment Variables

- `REACT_APP_DIFY_API_KEY`: Your Dify API key
- `REACT_APP_DIFY_API_URL`: Your Dify server URL (default: http://localhost:5000/v1)

## Building for Production

To build the app for production:

```bash
npm run build
```

The built files will be in the `build` directory.

## Docker Deployment

1. Build the Docker image:
```bash
docker build -t dify-chat-frontend .
```

2. Run the container:
```bash
docker run -p 3000:80 \
  -e REACT_APP_DIFY_API_KEY=your_api_key_here \
  -e REACT_APP_DIFY_API_URL=http://your-dify-server:5000/v1 \
  dify-chat-frontend
```

## License

MIT