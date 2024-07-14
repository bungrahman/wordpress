function restrict_limit_login($user_login, $user) {
    if (in_array($user_login, ['admin', 'adman'])) {
        return;
    }

    $sessions = WP_Session_Tokens::get_instance($user->ID);
    $sessions->destroy_others($sessions->get_token());
}

add_action('wp_login', 'restrict_limit_login', 10, 2);
