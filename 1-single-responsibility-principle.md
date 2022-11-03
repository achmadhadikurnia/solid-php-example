# Single Responsibility Principle (SRP)

## Original

```
<?php

class Page
{
    protected $title;

    public getPage($title)
    {
        return $this->title;
    }

    public function formatJson()
    {
        return json_encode($this->getTitle());
    }
}
```

## Refactored

```
<?php

class Page
{
    protected $title;

    public getPage($title)
    {
        return $this->title;
    }
}

class JsonPageFormatter
{
    public function format(Page $page)
    {
        return json_encode($page->getTitle());
    }
}
```
