function add_adman_role() {
    // Add new role "adman" with the same capabilities as the administrator role
    add_role(
        'adman',
        __('Adman'),
        get_role('administrator')->capabilities
    );
}
add_action('init', 'add_adman_role');



function remove_adman_role() {
    // Remove the "adman" role
    remove_role('adman');
}
add_action('init', 'remove_adman_role');

