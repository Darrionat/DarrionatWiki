---
description: A library for making the creation of plugins easier
---

# PluginLib

A project that aims to make the creation of plugins a faster and easier process. This project supports Minecraft 1.8.8-1.16.x.

## Maven

To add the library to your local Maven project, add the following to your pom.xml

#### Repository

```markup
<repository>
    <id>jitpack.io</id>
    <url>https://jitpack.io</url>
</repository>
```

#### Dependency

```markup
<dependency>
  <groupId>com.github.darrionat</groupId>
	<artifactId>PluginLib</artifactId>
	<version>version</version>
</dependency>
```

#### Shading

```markup
<build>
    <plugins>
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-shade-plugin</artifactId>
            <version>3.1.0</version>
            <configuration>
                <relocations>
                    <relocation>
                        <pattern>me.darrionat.pluginlib</pattern>
                        <!-- Make sure to change the package below -->
                        <shadedPattern>my.plugin.utils</shadedPattern>
                    </relocation>
                </relocations>
            </configuration>
            <executions>
                <execution>
                    <phase>package</phase>
                    <goals>
                        <goal>shade</goal>
                    </goals>
                </execution>
            </executions>
        </plugin>
    </plugins>
</build>
```

## Documentation

{% hint style="info" %}
The JavaDocs also contain plenty of information, make sure to read them before using a method!
{% endhint %}

todo: page links

