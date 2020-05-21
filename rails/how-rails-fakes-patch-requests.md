# Rails fakes PATCH requests as POST requests

Since web browsers can’t natively send PATCH requests (as required by the REST conventions),
Rails fakes it with a POST request and a hidden input field. When you inspect
HTML source for a form you will see this:
`<input name="_method" type="hidden" value="patch" />`
