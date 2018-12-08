# paginate

## How to use

```bash

composer require codeigniter-packages/installer
composer require codeigniter-packages/loader
composer require codeigniter-packages/paginate

```

```php

$this->load->package('codeigniter-packages/paginate');

$this->db->start_cache();

$this->paginate->filter(array('id','title'));
$this->db->from('tablename');

$this->db->stop_cache();
$this->db->order_by('id');

$this->paginate->get();

```