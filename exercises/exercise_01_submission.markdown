---
layout: default
title: Exercise Submission
---

# Exercise Submission Form

---

<form action="https://getsimpleform.com/messages?form_api_token=e864f49cd290bd127eeeb75cc92fd624" method="post" enctype="multipart/form-data">
  <!-- the redirect_to is optional, the form will redirect to the referrer on submission -->
<input type='hidden' name='redirect_to' value='http://retrography.github.io/data-management/exercises/' />

<input type='hidden' name='subject' value='an exercise submission' />

Name

<br /><input type='text' name='name' class='form-control' /><br />

McGill ID

<br /><input type='text' name='id' class='form-control' /><br />

Message

<br /><textarea name="message" class='form-control'></textarea><br />
<em>Please at least mention which exercise you are submitting.</emp><br />

File

<br /><input type='file' name='file' class='form-control' /><br />

<em>Please compress the file before uploading it. The server suppresses uncompressed scripts and text files.</emp><br />

<br /><input type='submit' value='Submit' class='form-control' />

</form>


