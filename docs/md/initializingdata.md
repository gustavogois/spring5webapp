[back](../../MyReadme.md)

# Initializing Data with Spring Framework

See ```bootstrap.DevBootstrap```.

1. Define the class as a component, using ```@Component``` annotation

2. Implements ```ApplicationListener<ContextRefreshedEvent>```, and override its method calling ```initData()```

3.  Autowire the repositories to add the objects