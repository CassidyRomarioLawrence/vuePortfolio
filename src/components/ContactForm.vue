<template>
    <div class="container-fluid mt-5">
    <form id="contact-form" method="POST" action="https://formspree.io/f/xqkjbrag" role="form">
        <div class="messages"></div>
        <div class="controls">
            <div class="row mt-5">
                <div class="col-md-6">
                    <div class="form-group">
                        <label for="form_name">Firstname *</label>
                        <input id="form_name" type="text" name="name" class="form-control"
                            placeholder="Please enter your firstname *" required="required"
                            data-error="Firstname is required." />
                        <div class="help-block with-errors"></div>
                    </div>
                </div>
                <div class="col-md-6">
                    <div class="form-group">
                        <label for="form_lastname">Lastname *</label>
                        <input id="form_lastname" type="text" name="surname" class="form-control"
                            placeholder="Please enter your lastname *" required="required"
                            data-error="Lastname is required." />
                        <div class="help-block with-errors"></div>
                    </div>
                </div>
            </div>
            <div class="row mt-5">
                <div class="col-md-6">
                    <div class="form-group">
                        <label for="form_email">Email *</label>
                        <input id="form_email" type="email" name="email" class="form-control"
                            placeholder="Please enter your email *" required="required"
                            data-error="Valid email is required." />
                        <div class="help-block with-errors"></div>
                    </div>
                </div>
                <div class="col-md-6">
                    <div class="form-group">
                        <label for="form_phone">Phone</label>
                        <input id="form_phone" type="tel" name="phone" class="form-control"
                            placeholder="Please enter your number" />
                        <div class="help-block with-errors"></div>
                    </div>
                </div>
            </div>
            <div class="row mt-5">
                <div class="col-md-12">
                    <div class="form-group">
                        <label for="form_message">Message *</label>
                        <textarea id="form_message" name="message" class="form-control" placeholder="Message for me *"
                            rows="4" required="required" data-error="Please leave a message."></textarea>
                        <div class="help-block with-errors"></div>
                    </div>
                </div>
                <div class="col-md-12 mt-3">
                    <input type="submit" class="btn btn-success btn-send" value="Send message" />
                </div>
            </div>
        </div>
    </form>
    </div>

    <div class="container mt-5">
        <div class="row">
            <div class="col-xs-12 col-md-4">
                <i class="bi bi-facebook"></i><a
                    href="https://www.facebook.com/cassidyromario.lawrence.7" target="_blank">Facebook | Cassidy Romario Lawrence</a>
            </div>
            <div class="col-xs-12 col-md-4">
                <i class="bi bi-linkedin"></i><a href="https://www.linkedin.com/in/cassidy-romario-lawrence-b671b21b8/"
                    target="_blank">LinkedIn | Cassidy Romario Lawrence</a>
            </div>
            <div class="col-xs-12 col-md-4">
                <i class="bi bi-instagram"></i><a href="https://www.instagram.com/cassidyromariolawrence/?next=%2F"
                    target="_blank">Instagram | @cassidyromariolawrence</a>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'ContactForm'
    }
</script>

<style scoped>
a{
    text-decoration: none;
    color: white;
}
form{
    font-weight: bold;
}
</style>