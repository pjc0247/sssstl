# sssstl

server-side-syncrhonized stl

```c++
sstd::vector<item> inventory("player3412.inventory");

inventory.push_back (item("long chicken"));

inventory.write_sync();

inventory.read_sync();

inventory.lock();
  inventory.push_back (item("fire dakdari"));
inventory.unlock();
```

__code__ <-> __stl interface__ <-> __query builder__ <-> __database adapter__ <-> __database__
