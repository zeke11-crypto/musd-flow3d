{
  "name": "Mezo MUSD Payment Verifier & CRM Router",
  "nodes": [
    {
      "parameters": { "httpMethod": "POST", "path": "mezo-musd-verified", "responseMode": "onReceived" },
      "name": "MUSD Checkout Webhook",
      "type": "n8n-nodes-base.webhook",
      "position": [240, 300]
    },
    {
      "parameters": {
        "url": "=https://explorer.test.mezo.org/api/v2/transactions/{{$json.body.txHash}}",
        "method": "GET"
      },
      "name": "Verify on Mezo Blockscout API",
      "type": "n8n-nodes-base.httpRequest",
      "position": [480, 300]
    }
  ]
}