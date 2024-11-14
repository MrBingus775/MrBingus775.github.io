---
layout: page
title: Contact
hide_title: true
permalink: /contact/
path: /contact/
description: "Want to get in touch with Pantheon Insights?"
order: 4
---

<div class="container mt-5 slide-in">
    <div class="" style="margin-top: 10vh;">
    <div class="row justify-content-center">
        <div class="col-lg-6">
            <h1 class="mb-4">Contact Pantheon Insights</h1>

            <p style="font-size: 1.2rem;">
              Please use the form below to inquire about Pantheon Insights speaking at your event, request consulting services, or address general queries: 
            </p>

            <br/>
            <form action="https://api.web3forms.com/submit" method="POST" style="font-size: 1.2rem;">

                <div class="mb-3">
                    <label for="name" class="form-label">Full Name</label>
                    <input type="text" class="form-control" name="name" id="name" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" name="email" id="email" required>
                </div>
                <div class="mb-3">
                    <label for="phone" class="form-label">Phone number <span style="color: grey;">(Optional)</span></label>
                    <input type="tel" class="form-control" id="phone" name="phone">
                </div>
                <div class="mb-3">
                    <label for="message" class="form-label">Your message</label>
                    <textarea class="form-control" id="message" name="message" rows="5" required></textarea>
                </div>

                <!-- access key directs to dzabelin@pantheoninsights.com -->
                <input type="hidden" name="access_key" value="e6b161a3-d66b-40bb-b92f-1c6f2132cd3a"/>
                <button class="primary-button" type="submit">Submit</button>
            
            </form>
            
            <script src="https://web3forms.com/client/script.js" async defer></script>

            <script>
                // On document ready, clear all the input forms above
                $(document).ready(function() {
                    document.getElementById('name').value = '';
                    document.getElementById('email').value = '';
                    document.getElementById('phone').value = '';
                    document.getElementById('message').value = '';
                });
            </script>
        </div>
    </div>
    <div class="" style="margin-top: 15vh;">
</div>
