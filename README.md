# Decidim::Jitsi_Meetings
[![Build Status](https://github.com/alabs/decidim-module-jitsi-videoconference/workflows/Ruby/badge.svg)](https://github.com/alabs/decidim-module-jitsi-meetings/actions)
[![Test Coverage](https://api.codeclimate.com/v1/badges/4ae591dc1f18df189316/test_coverage)](https://codeclimate.com/github/alabs/decidim-module-jitsi-meetings/test_coverage)
[![Maintainability](https://api.codeclimate.com/v1/badges/4ae591dc1f18df189316/maintainability)](https://codeclimate.com/github/alabs/decidim-module-jitsi-meetings/maintainability)

This module of [Decidim](https://decidim.org/) allows to deploy public or private videoconference rooms of any [jitsi](https://meet.jit.si/) server in participative processes and assemblies.

![decidim-jitsimeetings](decidim-jitsi.jpg)

## Installation

> NOTE: This module is ready to use but in Beta status. Feel free to report any bug! compatible and tested in versions Decidim 0.20 and 0.21.

1.- Add this line to your application's Gemfile:

```ruby
gem 'decidim-jitsi_meetings', git: 'https://github.com/alabs/decidim-module-jitsi-meetings.git'
```

2.- Run this rake tasks:

```bash
bundle install
rake decidim_jitsi_meetings:install:migrations
bundle exec rake db:migrate
```

## Usage

JitsiMeetings will be available as a Component for a Participatory Space (participative processes and assemblies)

![decidim-jitsi-deploy](module-jitsi-deploy.png)

To configure the module you only need to add three parameters, the server API access url, the jitsi server domain and the room name for the assembly or participatory process:

![decidim-jitsi-config](module-jitsi-config.png)

## Contributing

For instructions how to setup your development environment for Decidim, see [Decidim](https://github.com/decidim/decidim). Also follow Decidim's general instructions for development for this project as well.

## License

This engine is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
