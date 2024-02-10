# ForLeaf SQL Parser
An simple SQL parser written in PHP.

Just include the index PHP file and call the static parse function passing the query, like this:

$result = ForLeafParser::parse('select id,title from example_table limit 10');

The return object is an array with the query parameters:

array(
    'select' => array( 'id', 'title' ),
    'from' => 'example_table',
    'limit' => '10',
)

Thanks for read. 😁