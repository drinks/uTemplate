μTemplate is the simplest possible template renderer I could write in PHP.

**Usage:**

    /* template.php */
    <?php
    <h1><?=$title?></h1>
    <p><?=$content?></p>
    ?>
    ---
    /* myapp.php */
    include('class.utemplate.php');
    $context = array(
        "title" => "Hello, World!",
        "content" => "How's the weather?",
    )

    uTemplate::render($template_path, $context);
