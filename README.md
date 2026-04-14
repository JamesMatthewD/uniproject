# UniProject

Basic Next.js starter with frontend and backend API capabilities.

## Stack

- Next.js (App Router)
- React
- Built-in API routes via `app/api`

## Run Locally

```bash
npm install
npm run dev
```

Then open http://localhost:3000.

## API Endpoints

### Health Check

- Method: `GET`
- Path: `/api/health`

Response example:

```json
{
	"ok": true,
	"service": "uniproject-api",
	"timestamp": "2026-04-14T00:00:00.000Z"
}
```

### Echo Payload

- Method: `POST`
- Path: `/api/echo`
- Body: JSON

Request example:

```json
{
	"name": "James",
	"role": "student"
}
```

Response example:

```json
{
	"received": {
		"name": "James",
		"role": "student"
	},
	"message": "Echo from Next.js API route"
}
```
