# slim-rest-server
A simple and light framework to make a basic webserver

#step1:
git clone git@github.com:saifnoman/slim-rest-server.git

#step2:
```
create database iiuc;



--
-- Table structure for `tasks`
--
CREATE TABLE IF NOT EXISTS `tasks` (
  `id` int(11) NOT NULL,
  `task` varchar(200) NOT NULL,
  `status` tinyint(1) NOT NULL DEFAULT '1',
  `created_at` datetime NOT NULL DEFAULT CURRENT_TIMESTAMP
) ENGINE=InnoDB DEFAULT CHARSET=latin1;
 
ALTER TABLE `tasks` ADD PRIMARY KEY (`id`);
ALTER TABLE `tasks` MODIFY `id` int(11) NOT NULL AUTO_INCREMENT;

INSERT INTO `tasks` (`id`, `task`, `status`, `created_at`) VALUES
(1, 'Find bugs', 1, '2016-04-10 23:50:40'),
(2, 'Review code', 1, '2016-04-10 23:50:40'),
(3, 'Fix bugs', 1, '2016-04-10 23:50:40'),
(4, 'Refactor Code', 1, '2016-04-10 23:50:40'),
(5, 'Push to prod', 1, '2016-04-10 23:50:50’);
```
#step 3
In settings.php change this settings for your database

```
// database settings
        'db' => [
            "host" => "127.0.0.1",
            "dbname" => "iiuc",
            "user" => "root",
            "pass" => "719219"
        ],
```

#step4:
Open a browser and run http://localhost/iiuc_rest/todos

