# Nginx stub status Charts 
Application written in HTML5 and Javascript to represent the nginx stub status server-status data with graphs.

## Usage
Copy status.html to your server and run in a browser. The application automatically reads the data from /nginx_status.

Prerequisites
- Configure stub_status in location /nginx_status (https://nginx.org/libxslt/en/docs/http/ngx_http_stub_status_module.html)
```
location /nginx_status {
   stub_status;
}
```
- Make sure the computer you want to view the data has access to /nginx_status
- Edit status.html and set maxConections in line 23

It is advisable to run the status.html locally on the server to be monitored to avoid cross-domain problems (and prevent unwanted peeping).

For further information contact http://bernardosilva.com.br/#contato
