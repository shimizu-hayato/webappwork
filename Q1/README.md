# 解答

## POST

* curl

```
$ curl -F "lecture_sample_message[user]=moge" -F "lecture_sample_message[text]=mogemoge" -X POST https://tryout.sonicgarden.jp/lecture/sample/messages
```

* request

```
<html><body>You are being <a href="https://tryout.sonicgarden.jp/lecture/sample/messages/350">redirected</a>.</body></html>%
```

## GET

* curl

```
$ curl https://tryout.sonicgarden.jp/lecture/sample/messages/349 -X GET
```

* request

```
<!DOCTYPE html>
<html>
<head>
<script>
(省略)
</script>
<title>Samples</title>
<link rel="stylesheet" media="screen" href="/assets/lecture_sample-7c2401d58a372b5108ef153ec0175bb98d05e1148a51424a3b0e27745afd3106.css" />
<script src="/assets/lecture_sample-228b66fcfac63abe78efb648b8228df69cbc93ffbffdaf091a64b6c64b9f0662.js"></script>
<meta content='noindex,noarchive,nofollow' name='robots'>
<meta name="csrf-param" content="authenticity_token" />
<meta name="csrf-token" content="LDIAhXRWrS87SRoUiw/HQmz0dJ/PoSDjTMByxxWGrXDw6FDwKbDT08xMEXr0qLjK5uTM8xsLpzBCnz9G/uY/IQ==" />
</head>
<body>
<div class='container'>
<div class='row'>
<div class='col-md-8 col-md-offset-2'>
<h1>Show lecture_sample_message</h1>
<p id='notice'></p>
<p>
<b>User:</b>
hage
</p>
<p>
<b>Text:</b>
hagehage
</p>
<a href="/lecture/sample/messages/349/edit">Edit</a>
|
<a href="/lecture/sample/messages">Back</a>

</div>
</div>
</div>
</body>
</html>
```
## PUT

* curl

```
$ curl -F "lecture_sample_message[user]=hage" -F "lecture_sample_message[text]=hagehage" -X PUT "https://tryout.sonicgarden.jp/lecture/sample/messages/349"
```

* request

```
<html><body>You are being <a href="https://tryout.sonicgarden.jp/lecture/sample/messages/349">redirected</a>.</body></html>%
```
## DELETE

* curl

```
$ curl https://tryout.sonicgarden.jp/lecture/sample/messages/350 -X DELETE
```

* request

```
<html><body>You are being <a href="https://tryout.sonicgarden.jp/lecture/sample/messages">redirected</a>.</body></html>%
```