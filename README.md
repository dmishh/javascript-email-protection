# Javascript email protection (JEP)

Perfectly protects your email from bots that are scanning HTML without executing JavaScript.

## Usage in HTML:

### Simple

    <script type="text/javascript">jep_link("example.com", "mailbox")</script>
    => writes to DOM: <a href="mailto:mailbox@example.com">mail@example.com</a>

### Custom link text

    <script type="text/javascript">jep_link("example.com", "mailbox", "my email")</script>
    => writes to DOM: <a href="mailto:mailbox@example.com">my email</a>

### Return generated HTML instead of printing it to DOM

    <script type="text/javascript">jep_link("example.com", "mailbox", "my email", true)</script>
    => returns as string: <a href="mailto:mailbox@example.com">my email</a>