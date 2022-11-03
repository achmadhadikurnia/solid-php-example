# Dependency Inversion Principle (DIP)

## Original

```
<?php

class MySqlConnection
{
    public function connect() {}
}

class PageLoader
{
    private $dbConnection;

    public function __construct(MySqlConnection $dbConnection)
    {
        $this->dbConnection = $dbConnection;
    }
}
```

## Refactored

```
<?php

interface DbConnectionInterface
{
    public function connect();
}

class MySqlConnection implements DbConnectionInterface
{
    public function connect() {}
}

class PageLoader
{
    private $dbConnection;

    public function __construct(DbConnectionInterface $dbConnection)
    {
        $this->dbConnection = $dbConnection;
    }
}
```
