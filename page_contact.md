---
layout: page
title: Contact
hide_title: true
permalink: /contact/
path: /contact/
order: 4
---

<div class="container mt-5">
    <div class="row justify-content-center">
        <div class="col-lg-6">
            <h2 class="mb-4">Contact Pantheon Insights</h2>

            <p>
              Please use the form below to inquire about Pantheon Insights speaking at your event, request consulting services, or address general queries: 
            </p>

            <br/>
            <form action="https://api.web3forms.com/submit" method="POST">

                <div class="mb-3">
                    <label for="name" class="form-label">Full Name</label>
                    <input type="text" class="form-control" name="name" id="name" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" name="email" id="email" required>
                </div>
                <div class="mb-3">
                    <label for="phone" class="form-label">Phone number</label>
                    <input type="tel" class="form-control" id="phone" required>
                </div>
                <div class="mb-3">
                    <label for="message" class="form-label">Your message</label>
                    <textarea class="form-control" id="message" rows="5" required></textarea>
                </div>

                <input type="hidden" name="access_key" value="ff2d64e5-760e-40d5-bace-a9df6f0ddf1e">
                <button class="btn btn-primary" type="submit">Submit</button>
            
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
</div>
