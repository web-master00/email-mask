# Email Mask

A small Express service that masks the local part of an email address. `john@example.com` becomes `j***@example.com`. The domain is left unchanged. Invalid input returns an error string instead of a masked address.

## Requirements

- Node.js 18 or newer

## Run

```bash
npm install
npm start
```

The server listens on port 3000.

## API

`GET /functions/maskEmail` returns a short description of the function.

`POST /functions/maskEmail` with a JSON body:

```json
{ "input": "john@example.com" }
```

Response:

```json
{ "output": "j***@example.com" }
```
