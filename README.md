<!--lint disable double-link-->
> 说明：基于 [Awesome-fastapi](https://github.com/mjhea0/awesome-fastapi)项目翻译而来，感谢原作者的贡献。

# Awesome FastAPI | [![Awesome](https://awesome.re/badge-flat.svg)](https://github.com/sindresorhus/awesome)

> 与 FastAPI 相关的精选清单

[FastAPI](https://fastapi.tiangolo.com/) 是一个用于构建 API 的现代、快速（高性能）的 web 框架，非常适合构建 RESTful API.

## 内容

- [第三方扩展](#third-party-extensions)
  - [Admin](#admin)
  - [Auth](#auth)
  - [Databases](#databases)
  - [Developer Tools](#developer-tools)
  - [Email](#email)
  - [Utils](#utils)
- [Resources](#resources)
  - [Official Resources](#official-resources)
  - [External Resources](#external-resources)
  - [Podcasts](#podcasts)
  - [Articles](#articles)
  - [Tutorials](#tutorials)
  - [Talks](#talks)
  - [Videos](#videos)
  - [Courses](#courses)
  - [Best Practices](#best-practices)
- [Hosting](#hosting)
  - [PaaS](#paas)
  - [IaaS](#iaas)
  - [Serverless](#serverless)
- [Projects](#projects)
  - [Boilerplate](#boilerplate)
  - [Docker Images](#docker-images)
  - [Open Source Projects](#open-source-projects)
- [Sponsors](#sponsors)

## Third-Party Extensions

### Admin

- [FastAPI Admin](https://github.com/fastapi-admin/fastapi-admin) - 功能管理面板，提供用于对数据执行 CRUD 操作的用户界面。目前仅适用于 Tortoise ORM。
- [Piccolo Admin](https://github.com/piccolo-orm/piccolo_admin) - 一个强大而现代的管理 GUI，使用 Piccolo ORM。
- [SQLAlchemy Admin](https://github.com/aminalaee/sqladmin) - 适用于 SQLAlchemy 模型的 FastAPI/Starlette 管理面板。

### Auth

- [AuthX](https://github.com/yezz123/AuthX) - 用于FastAPI的可定制的认证和Oauth2管理。
- [FastAPI Auth](https://github.com/dmontagu/fastapi-auth) - 支持OAuth2密码、JWT访问和刷新令牌的可插拔式的认证。
- [FastAPI Azure Auth](https://github.com/Intility/fastapi-azure-auth) - 为你的API提供Azure AD认证，支持单租户和多租户。
- [FastAPI Cloud Auth](https://github.com/tokusumi/fastapi-cloudauth) - FastAPI和云认证服务 (AWS Cognito, Auth0, Firebase Authentication) 之间的简单集成。.
- [FastAPI Login](https://github.com/MushroomMaula/fastapi_login) - 账号管理和认证 (基于 [Flask-Login](https://github.com/maxcountryman/flask-login)).
- [FastAPI JWT Auth](https://github.com/IndominusByte/fastapi-jwt-auth) - JWT 认证 (基于 [Flask-JWT-Extended](https://github.com/vimalloc/flask-jwt-extended)).
- [FastAPI Permissions](https://github.com/holgi/fastapi-permissions) - Row-level 权限控制.
- [FastAPI Security](https://github.com/jacobsvante/fastapi-security) - 结合FastAPI的依赖项，实施认证和授权。
- [FastAPI Simple Security](https://github.com/mrtolkien/fastapi_simple_security) - 通过路径操作，来管理开箱即用的API密钥安全。
- [FastAPI Users](https://github.com/fastapi-users/fastapi-users) - 账户管理、认证、授权。

### Databases

#### ORMs

- [FastAPI SQLAlchemy](https://github.com/mfreeborn/fastapi-sqlalchemy) - FastAPI 和 [SQLAlchemy](https://www.sqlalchemy.org/) 之间的简单集成。
- [Fastapi-SQLA](https://github.com/dialoguemd/fastapi-sqla) - SQL Alchemy 扩展用于快速 API，支持分页、异步和 pytest。
- [FastAPIwee](https://github.com/Ignisor/FastAPIwee) - 基于 [PeeWee](https://github.com/coleifer/peewee) 模型创建 REST API 的简单方法
- [GINO](https://github.com/python-gino/gino) - 一个基于Python异步，建立在 SQLAlchemy 核心之上轻量级异步 ORM。
  - [FastAPI Example](https://github.com/leosussan/fastapi-gino-arq-uvicorn)
- [ORM](https://github.com/encode/orm) - 一个异步 ORM.
- [ormar](https://collerek.github.io/ormar/) - Ormar 是一个异步 ORM，可以直接用于FastAPI请求和响应，因此你只需要维护一套模型，包含 Alembic 迁移
  - [FastAPI Example](https://collerek.github.io/ormar/fastapi/) - 在ormar使用FastAPI框架.
- [Piccolo](https://github.com/piccolo-orm/piccolo) - 一个异步ORM和查询生成器，支持Postgres和SQLite，带有功能 (迁移、安全等).
  - [FastAPI Examples](https://github.com/piccolo-orm/piccolo_examples) - 在Piccolo 使用FastAPI框架.
- [Prisma Client Python](https://github.com/RobertCraigie/prisma-client-py) - 一个由Pydantic提供的自动生成的、全部类型安全的ORM，并为你的模式专门定制 - 支持SQLite、PostgreSQL、MySQL、MongoDB、MariaDB等。
  - [FastAPI Example](https://github.com/RobertCraigie/prisma-client-py/tree/main/examples/fastapi-basic) - FastAPI 示例
- [Tortoise ORM](https://tortoise.github.io) - 一个易于使用的异步 ORM（对象关系映射器），灵感来自Django
  - [FastAPI Example](https://tortoise.github.io/examples/fastapi.html) - 一个 Tortoise-ORM FastAPI 集成的例子.
  - [Tutorial: Setting up Tortoise ORM with FastAPI](https://web.archive.org/web/20200523174158/https://robwagner.dev/tortoise-fastapi-setup/)
  - [Aerich](https://github.com/tortoise/aerich) - Tortoise ORM 迁移工具.
- [SQLModel](https://sqlmodel.tiangolo.com/) - (由Pydantic和SQLAlchemy驱动)是一个用于与Python代码交互的SQL数据库的库，具有Python对象。

#### Query Builders 

- [asyncpgsa](https://github.com/CanopyTax/asyncpgsa) - 一个用于 [SQLAlchemy Core](https://docs.sqlalchemy.org/en/latest/core/) 的 [asyncpg](https://github.com/MagicStack/asyncpg)的包装器。
- [Databases](https://github.com/encode/databases) - 异步sql查询构建器，基于 [SQLAlchemy Core](https://docs.sqlalchemy.org/en/latest/core/) 表达式语言。

#### ODMs 

- [Beanie](https://github.com/roman-right/beanie) - 用于MongoDB的异步Python ODM，基于 [Motor](https://motor.readthedocs.io/en/stable/) 和 [Pydantic](https://pydantic-docs.helpmanual.io/), 支持数据和模式迁移。
- [MongoEngine](http://mongoengine.org/) - 一个用于Python的MongoDB文档对象映射器（类似于ORM，但用于文档数据库）。
- [Motor](https://motor.readthedocs.io/) -  异步MongoDB的Python驱动程序。
- [ODMantic](https://art049.github.io/odmantic/) - AsyncIO MongoDB ODM 集成 [Pydantic](https://pydantic-docs.helpmanual.io/)

#### Other Tools (其他工具)

- [Pydantic-SQLAlchemy](https://github.com/tiangolo/pydantic-sqlalchemy) - 将SQLAlchemy模型转换为 [Pydantic](https://pydantic-docs.helpmanual.io/) 模型。
- [FastAPI-CamelCase](https://nf1s.github.io/fastapi-camelcase/) - 利用 [Pydantic](https://pydantic-docs.helpmanual.io/) 的CamelCase JSON支持。
  - [CamelCase Models with FastAPI and Pydantic](https://medium.com/analytics-vidhya/camel-case-models-with-fast-api-and-pydantic-5a8acb6c0eee) - Accompanying blog post from the author of the extension. 随之而来的作者扩展的博客文章。

### Developer Tools (开发者工具)

- [FastAPI Code Generator](https://github.com/koxudaxi/fastapi-code-generator) - 从OpenAPI文件创建FastAPI应用程序，从而实现模式驱动的开发。
- [FastAPI Client Generator](https://github.com/dmontagu/fastapi_client) -  基于OpenAPI规范生成一个mypy和IDE友好的API客户端。
- [FastAPI MVC](https://github.com/fastapi-mvc/fastapi-mvc) - 开发人员生产力工具，用于制作高质量的FastAPI生产就绪API。
- [FastAPI Profiler](https://github.com/sunhailin-Leo/fastapi_profiler) - 一个基于joerick/pyinstrument，检查你的服务性能的FastAPI中间件。
- [FastAPI Versioning](https://github.com/DeanWay/fastapi-versioning) - API 的版本控制.
- [Jupyter Notebook REST API](https://github.com/Invictify/Jupter-Notebook-REST-API) - 运行你的Jupyter笔记本作为RESTful API端点。
- [Manage FastAPI](https://github.com/ycd/manage-fastapi) - CLI 工具，用于生成和管理 FastAPI 项目。
- [msgpack-asgi](https://github.com/florimondmanca/msgpack-asgi) - 自动 [MessagePack](https://msgpack.org/) 内容协商。

### Email (邮箱)

- [FastAPI Mail](https://github.com/sabuhish/fastapi-mail) - 轻量级邮件系统，用于发送电子邮件和附件（单个和批量）。

### Utils (工具)

- [ASGI Correlation ID](https://github.com/snok/asgi-correlation-id) - 请求ID日志中间件。
- [FastAPI Cache](https://github.com/comeuplater/fastapi_cache) - 一个简单的轻量级缓存系统。
- [FastAPI Cache](https://github.com/long2ice/fastapi-cache) - 一个用于缓存FastAPI响应和函数结果的工具，支持Redis，Memcached，DynamoDB和内存后端。
- [FastAPI Chameleon](https://github.com/mikeckennedy/fastapi-chameleon) - 增加了Chameleon模板语言到FastAPI的集成。
- [FastAPI Contrib](https://github.com/identixone/fastapi_contrib) - 一组有观点的实用程序：分页，身份验证中间件，权限，自定义异常处理程序，MongoDB支持和Opentracing中间件。
- [FastAPI CRUDRouter](https://github.com/awtkns/fastapi-crudrouter) - 一个自动创建和记录CRUD路由的FastAPI路由器，用于你的模型。
- [FastAPI Events](https://github.com/melvinkcx/fastapi-events) - 用于FastAPI和Starlette的异步事件调度/处理库。
- [FastAPI FeatureFlags](https://github.com/Pytlicek/fastapi-featureflags) - 简单的FastAPI功能标志的实现。
- [FastAPI Jinja](https://github.com/AGeekInside/fastapi-jinja) - 增加了Jinja模板语言到FastAPI的集成。
- [FastAPI Lazy](https://github.com/yezz123/fastapi-lazy) - 一个懒惰的包，用于使用FastAPI启动你的项目。
- [FastAPI Limiter](https://github.com/long2ice/fastapi-limiter) - 一个用于限制FastAPI请求的工具。
- [FastAPI MQTT](https://github.com/sabuhish/fastapi-mqtt) - 一个 MQTT 协议的扩展。
- [FastAPI Opentracing](https://github.com/wesdu/fastapi-opentracing) - Opentracing 中间件和数据库跟踪支持FastAPI。
- [FastAPI Pagination](https://github.com/uriyyo/fastapi-pagination) - FastAPI 分页。
- [FastAPI Plugins](https://github.com/madkote/fastapi-plugins) - Redis 和 Scheduler 插件。
- [FastAPI ServiceUtils](https://github.com/skallfass/fastapi_serviceutils) - 用于创建API服务的生成器。
- [FastAPI SocketIO](https://github.com/pyropy/fastapi-socketio) - FastAPI 和 SocketIO 的简单集成。
- [FastAPI Utilities](https://github.com/dmontagu/fastapi-utils) - 重用的实用程序：基于类的视图，响应推断路由器，定期任务，计时中间件，SQLAlchemy会话，OpenAPI规范简化。
- [FastAPI Websocket Pub/Sub](https://github.com/authorizon/fastapi_websocket_pubsub) - Websocket pub/sub 模式，使其在云中的任何地方都可以轻松访问和扩展。
- [FastAPI Websocket RPC](https://github.com/authorizon/fastapi_websocket_rpc) - 通过 Websockets 的 RPC（双向 JSON RPC）变得简单、健壮和生产就绪。
- [OpenTelemetry FastAPI Instrumentation](https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-fastapi) - [OpenTelemetry](https://opentelemetry.io/) 是一个开放的自动跟踪工具包，用于监视应用程序的性能和可用性。
- [Prerender Python Starlette](https://github.com/BeeMyDesk/prerender-python-starlette) - 一个用于预渲染爬虫的中间件。
- [Prometheus FastAPI Instrumentator](https://github.com/trallnag/prometheus-fastapi-instrumentator) - 一个可配置和模块化的 Prometheus Instrumentator 用于你的 FastAPI 应用程序。
- [SlowApi](https://github.com/laurents/slowapi) - 限速器（基于 [Flask-Limiter](https://flask-limiter.readthedocs.io)）。
- [Starlette Context](https://github.com/tomwojcik/starlette-context) - 允许你在项目的任何地方存储和访问请求数据，对于日志记录很有用。
- [Starlette Exporter](https://github.com/stephenhillier/starlette_exporter) - 一个用于 FastAPI 和 Starlette 的 Prometheus 集成。
- [Starlette OpenTracing](https://github.com/acidjunk/starlette-opentracing) - 对于 Starlette 和 FastAPI 的 Opentracing 支持。
- [Starlette Prometheus](https://github.com/perdy/starlette-prometheus) - FastAPI 和 Starlette 的 Prometheus 集成。
- [Strawberry GraphQL](https://github.com/strawberry-graphql/strawberry) - 一个基于dataclasses的 Python GraphQL 库。

## Resources 

### Official Resources and Tutorials (官方资源和教程)

- [Documentation](https://fastapi.tiangolo.com/) - FastAPI 官方链接。
- [Tutorial](https://fastapi.tiangolo.com/tutorial/) - FastAPI 官方教程，逐步展示了如何使用 FastAPI 的大部分功能。
- [Source Code](https://github.com/tiangolo/fastapi) - FastAPI 的源代码。
- [Discord](https://discord.com/invite/VQjSZaeJmf) - 与其他 FastAPI 用户聊天。

### External Resources (外部资源)

- [TestDriven.io FastAPI](https://testdriven.io/blog/topics/fastapi/) - 多篇专注于开发和测试生产就绪的 RESTful API、提供机器学习模型等的 FastAPI 特定文章。

### Podcasts (播客)

- [Build The Next Generation Of Python Web Applications With FastAPI](https://www.pythonpodcast.com/fastapi-web-application-framework-episode-259/) - 这个播客的第 259 集 [Podcast Init](https://www.pythonpodcast.com/), FastAPI 的创建者 [Sebastián Ramirez](https://tiangolo.com/) 分享了他创建 FastAPI 的动机以及它的工作原理。
- [FastAPI on PythonBytes](https://pythonbytes.fm/episodes/show/123/time-to-right-the-py-wrongs?time_in_sec=855) - 不错的项目概述。

### Articles (文章)

- [FastAPI has Ruined Flask Forever for Me](https://towardsdatascience.com/fastapi-has-ruined-flask-forever-for-me-73916127da)
- [Why we switched from Flask to FastAPI for production machine learning](https://medium.com/@calebkaiser/why-we-switched-from-flask-to-fastapi-for-production-machine-learning-765aab9b3679) - 深入了解为什么你可能想从 Flask 迁移到 FastAPI。

### Tutorials (教程)

- [Async SQLAlchemy with FastAPI](https://stribny.name/blog/fastapi-asyncalchemy/) - 学习如何异步使用 SQLAlchemy。
- [Build and Secure an API in Python with FastAPI](https://blog.yezz.me/blog/Build-and-Secure-an-API-in-Python-with-FastAPI) - 保护和维护基于 FastAPI 和 SQLAlchemy 的 API。
- [Deploy a Dockerized FastAPI App to Google Cloud Platform](https://towardsdatascience.com/deploy-a-dockerized-fastapi-app-to-google-cloud-platform-24f72266c7ef) - 一个简短的指南，用于使用 Cloud Run 和 SQL 实例将 Docker 化的 Python 应用部署到 Google Cloud Platform。
- [Deploy Machine Learning Models with Keras, FastAPI, Redis and Docker](https://medium.com/analytics-vidhya/deploy-machine-learning-models-with-keras-fastapi-redis-and-docker-4940df614ece)
- [Deploying Iris Classifications with FastAPI and Docker](https://towardsdatascience.com/deploying-iris-classifications-with-fastapi-and-docker-7c9b83fdec3a) - 将 FastAPI 应用程序 Docker 化。
- [Developing and Testing an Asynchronous API with FastAPI and Pytest](https://testdriven.io/blog/fastapi-crud/) - 使用 TDD 开发和测试使用 FastAPI、Postgres、Pytest 和 Docker 的异步 API。
- [FastAPI for Flask Users](https://amitness.com/2020/06/fastapi-vs-flask/) - 通过与 Flask 的并排代码比较学习 FastAPI。
- [FastAPI Microservice Patterns](https://florian-kromer.medium.com/fastapi-microservice-patterns-3052c1241019) - 一个包含微服务模式示例实现的博客系列。
  - [Local Development Environment](https://florian-kromer.medium.com/fastapi-microservice-patterns-local-development-environment-12182e786f1c) - 简而言之，Skaffold、docker、kubectl 和 minikube。
  - [Service discovery in Container Orchestration Platforms](https://florian-kromer.medium.com/fastapi-microservice-patterns-service-discovery-in-container-orchestration-platforms-290c00d1ad8) - 解释了在 Kubernetes 中启用 FastAPI 服务通信。
  - [Asynchronous Communication](https://florian-kromer.medium.com/fastapi-microservice-patterns-asynchronous-communication-45a3b68f8bb8) - 通过消息使服务松耦合。
  - [Application Monitoring](https://medium.com/swlh/fastapi-microservice-patterns-application-monitoring-49fcb7341d9a) - 使用 Prometheus 和 Grafana 监控应用程序指标。
  - [Serverless Deployment](https://medium.com/swlh/fastapi-microservice-serverless-deployment-41a6d21e5cb3) - 关于 FastAPI 与 Kubernetes 原生 FaaS 平台兼容性的当前状态。
- [Getting started with GraphQL in Python with FastAPI and Ariadne](https://blog.yezz.me/blog/Getting-started-with-GraphQL-in-Python-with-FastAPI-and-Ariadne) - 使用 FastAPI、GraphQL 和 Ariadne 生成一个 FullStack 沙盒。
- [How to monitor your FastAPI service](https://guitton.co/posts/fastapi-monitoring) - 解释了如何使用 OpenTelemetry 和 Datadog/Jaeger 实现应用程序性能监控（APM）。
- [Implementing FastAPI Services – Abstraction and Separation of Concerns](https://camillovisini.com/article/abstracting-fastapi-services/) - FastAPI 应用程序和服务结构，以实现更易维护的代码库。
- [Introducing FARM Stack - FastAPI, React, and MongoDB](https://www.mongodb.com/developer/languages/python/farm-stack-fastapi-react-mongodb/) - 一个完整的 FastAPI Web 应用程序栈的入门指南。
- [Multitenancy with FastAPI, SQLAlchemy and PostgreSQL](https://mergeboard.com/blog/6-multitenancy-fastapi-sqlalchemy-postgresql/) - 学习如何使 FastAPI 应用程序具有多租户功能。
- [Porting Flask to FastAPI for ML Model Serving](https://www.pluralsight.com/tech-blog/porting-flask-to-fastapi-for-ml-model-serving/) - 一个 Flask 和 FastAPI 模型服务的对比。
- [Real-time data streaming using FastAPI and WebSockets](https://stribny.name/blog/2020/07/real-time-data-streaming-using-fastapi-and-websockets/) - 学习如何将数据从 FastAPI 直接流式传输到实时图表中。
- [Running FastAPI applications in production](https://stribny.name/blog/fastapi-production/) - 使用 Gunicorn 和 systemd 进行生产部署。
- [Serving Machine Learning Models with FastAPI in Python](https://medium.com/@8B_EC/tutorial-serving-machine-learning-models-with-fastapi-in-python-c1a27319c459) - 使用 FastAPI 快速轻松地部署和提供 Python 中的机器学习模型作为 RESTful API。
- [Streaming video with FastAPI](https://stribny.name/blog/fastapi-video/) - 学习如何提供视频流。
- [Using Hypothesis and Schemathesis to Test FastAPI](https://testdriven.io/blog/fastapi-hypothesis/) - 使用属性基础测试来测试 FastAPI。

### Talks (演讲)

- [PyConBY 2020: Serve ML models easily with FastAPI](https://www.youtube.com/watch?v=z9K5pwb0rt8) - From the talk by Sebastian Ramirez you will learn how to easily build a production-ready web (JSON) API for your ML models with FastAPI, including best practices by default.
- [PyCon UK 2019: FastAPI from the ground up](https://www.youtube.com/watch?v=3DLwPcrE5mA) - This talk shows how to build a simple REST API for a database from the ground up using FastAPI.

### Videos (视频)

- [Building a Stock Screener with FastAPI](https://www.youtube.com/watch?v=5GorMC2lPpk) - A you build a web-based stock screener with FastAPI, you'll be introduced to many of FastAPI's features, including Pydantic models, dependency injection, background tasks, and SQLAlchemy integration.
- [Building Web APIs Using FastAPI](https://www.youtube.com/watch?v=Pe66M8mn-wA) - Use FastAPI to build a web application programming interface (RESTful API).
- [FastAPI - A Web Framework for Python](https://www.youtube.com/watch?v=PUhio8CprhI&list=PL5gdMNl42qynpY-o43Jk3evfxEKSts3HS) - See how to do numeric validations with FastAPI.
- [FastAPI vs. Django vs. Flask](https://www.youtube.com/watch?v=9YBAOYQOzWs) - Which framework is best for Python in 2020? Which uses async/await the best? Which is the fastest?
- [Serving Machine Learning Models As API with FastAPI](https://www.youtube.com/watch?v=mkDxuRvKUL8) - Build a machine learning API with FastAPI.

### Courses (课程)

- [Test-Driven Development with FastAPI and Docker](https://testdriven.io/courses/tdd-fastapi/) - Learn how to build, test, and deploy a text summarization microservice with Python, FastAPI, and Docker.
- [Modern APIs with FastAPI and Python](https://training.talkpython.fm/courses/getting-started-with-fastapi) - A course designed to get you creating new APIs running in the cloud with FastAPI quickly.
- [Full Web Apps with FastAPI Course](https://training.talkpython.fm/courses/full-html-web-applications-with-fastapi) - You'll learn to build full web apps with FastAPI, equivalent to what you can do with Flask or Django.
- [The Definitive Guide to Celery and FastAPI](https://testdriven.io/courses/fastapi-celery/) - Learn how to add Celery to a FastAPI application to provide asynchronous task processing.

### Best Practices (最佳实践)

- [FastAPI Best Practices](https://github.com/zhanymkanov/fastapi-best-practices) - Collection of best practices in a GitHub repo.

## Hosting

### PaaS (平台即服务)

(Platforms-as-a-Service)

- [Heroku](https://www.heroku.com/) ([Step-by-step tutorial](https://tutlinks.com/create-and-deploy-fastapi-app-to-heroku/), [ML model on Heroku tutorial](https://testdriven.io/blog/fastapi-machine-learning/))
- [AWS Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/)
- [Google App Engine](https://cloud.google.com/appengine/)
- [Microsoft Azure App Service](https://azure.microsoft.com/en-us/products/app-service/)
- [Deta](https://www.deta.sh/) ([example](https://dev.to/athulcajay/fastapi-deta-ni5))

### IaaS (基础设施即服务)

(Infrastructure-as-a-Service)

- [AWS EC2](https://aws.amazon.com/ec2/)
- [Google Compute Engine](https://cloud.google.com/compute/)
- [Digital Ocean](https://www.digitalocean.com/)
- [Linode](https://www.linode.com/)

### Serverless (无服务器)

Frameworks:

- [Chalice](https://github.com/aws/chalice)
- [Mangum](https://mangum.io/) - Adapter for running ASGI applications with AWS Lambda and API Gateway.
- [Vercel](https://vercel.com/) - (formerly Zeit) ([example](https://github.com/paul121/fastapi-zeit-now)).

Compute:

- [AWS Lambda](https://aws.amazon.com/lambda/) ([tutorial](https://iwpnd.pw/articles/2020-01/deploy-fastapi-to-aws-lambda), [code](https://github.com/iwpnd/fastapi-aws-lambda-example))
- [Google Cloud Functions](https://cloud.google.com/functions/)
- [Azure Functions](https://azure.microsoft.com/en-us/products/functions/)
- [Google Cloud Run](https://cloud.google.com/run) ([example](https://github.com/anthonycorletti/cloudrun-fastapi))

## Projects 

### Boilerplate

- [Full Stack FastAPI and PostgreSQL - Base Project Generator](https://github.com/tiangolo/full-stack-fastapi-postgresql) - Full stack, modern web application generator, which includes FastAPI, PostgreSQL, Docker, Celery, Vue frontend, automatic HTTPS and more (developed by the creator of FastAPI, [Sebastián Ramírez](https://github.com/tiangolo)).
- [FastAPI and Tortoise ORM](https://github.com/prostomarkeloff/fastapi-tortoise) - Powerful but simple template for web APIs w/ FastAPI (as web framework) and Tortoise-ORM (for working via database without headache).
- [FastAPI Model Server Skeleton](https://github.com/eightBEC/fastapi-ml-skeleton) - Skeleton app to serve machine learning models production-ready.
- [cookiecutter-spacy-fastapi](https://github.com/microsoft/cookiecutter-spacy-fastapi) - Quick deployments of spaCy models with FastAPI.
- [cookiecutter-fastapi](https://github.com/arthurhenrique/cookiecutter-fastapi) - Cookiecutter template for FastAPI projects using: Machine Learning, Poetry, Azure Pipelines and pytest.
- [openapi-python-client](https://github.com/openapi-generators/openapi-python-client) - Generate modern FastAPI Python clients (via FastAPI) from OpenAPI.
- [Pywork](https://github.com/vutran1710/YeomanPywork) - [Yeoman](https://yeoman.io/) generator to scaffold a FastAPI app.
- [fastapi-gino-arq-uvicorn](https://github.com/leosussan/fastapi-gino-arq-uvicorn) - Template for a high-performance async REST API, in Python. FastAPI + GINO + Arq + Uvicorn (w/ Redis and PostgreSQL).
- [FastAPI and React Template](https://github.com/Buuntu/fastapi-react) - Full stack cookiecutter boilerplate using FastAPI, TypeScript, Docker, PostgreSQL, and React.
- [FastAPI Nano](https://github.com/rednafi/fastapi-nano) - Simple FastAPI template with factory pattern architecture.
- [FastAPI template](https://github.com/s3rius/FastAPI-template) - Flexible, lightweight FastAPI project generator. It includes support for SQLAlchemy, multiple databases, CI/CD, Docker, and Kubernetes.
- [FastAPI on Google Cloud Run](https://github.com/anthonycorletti/cloudrun-fastapi) - Boilerplate for API building with FastAPI, SQLModel, and Google Cloud Run.
- [FastAPI with Firestore](https://github.com/anthonycorletti/firestore-fastapi) - Boilerplate for API building with FastAPI and Google Cloud Firestore.
- [fastapi-alembic-sqlmodel-async](https://github.com/jonra1993/fastapi-alembic-sqlmodel-async) - This is a project template which uses FastAPI, Alembic, and async SQLModel as ORM.
- [fastapi-starter-project](https://github.com/mirzadelic/fastapi-starter-project) - A project template which uses FastAPI, SQLModel, Alembic, Pytest, Docker, GitHub Actions CI.

### Docker Images

- [inboard](https://github.com/br3ndonland/inboard) - Docker images to power your FastAPI apps and help you ship faster.
- [uvicorn-gunicorn-fastapi-docker](https://github.com/tiangolo/uvicorn-gunicorn-fastapi-docker) - Docker image with Uvicorn managed by Gunicorn for high-performance FastAPI web applications in Python 3.7 and 3.6 with performance auto-tuning.
- [uvicorn-gunicorn-poetry](https://github.com/max-pfeiffer/uvicorn-gunicorn-poetry) - This Docker image provides a platform to run FastAPI using Gunicorn with Uvicorn workers. It provides Poetry for managing dependencies and setting up a virtual environment in the container.
- [uvicorn-poetry](https://github.com/max-pfeiffer/uvicorn-poetry) - This Docker image provides a platform to run FastAPI with Uvicorn on Kubernetes container orchestration system. It provides Poetry for managing dependencies and setting up a virtual environment in the container.

### Open Source Projects

- [Astrobase](https://github.com/anthonycorletti/astrobase) - Simple, fast, and secure deployments anywhere.
- [Awesome FastAPI Projects](https://github.com/Kludex/awesome-fastapi-projects) - Organized list of projects that use FastAPI.
- [Bitcart](https://github.com/bitcartcc/bitcart) - Platform for merchants, users and developers which offers easy setup and use.
- [Bali](https://github.com/bali-framework/bali) - Simplify Cloud Native Microservices development base on FastAPI and gRPC.
- [Bunnybook](https://github.com/pietrobassi/bunnybook) - A tiny social network built with FastAPI, React+RxJs, Neo4j, PostgreSQL, and Redis.
- [Coronavirus-tg-api](https://github.com/egbakou/coronavirus-tg-api) - API for tracking the global coronavirus (COVID-19, SARS-CoV-2) outbreak.
- [Dispatch](https://github.com/Netflix/dispatch) - Manage security incidents.
- FastAPI CRUD Example:
  - [Async flavor](https://github.com/testdrivenio/fastapi-crud-async)
  - [Sync Flavor](https://github.com/testdrivenio/fastapi-crud-sync)
- [DogeAPI](https://github.com/yezz123/DogeAPI) - API with high performance to create a simple blog and CRUD with OAuth2PasswordBearer.
- [FastAPI Websocket Broadcast](https://github.com/kthwaite/fastapi-websocket-broadcast) - Websocket 'broadcast' demo.
- [FastAPI with Celery, RabbitMQ, and Redis](https://github.com/GregaVrbancic/fastapi-celery) - Minimal example utilizing FastAPI and Celery with RabbitMQ for task queue, Redis for Celery backend, and Flower for monitoring the Celery tasks.
- [JeffQL](https://github.com/yezz123/JeffQL/) - Simple authentication and login API using GraphQL and JWT.
- [JSON-RPC Server](https://github.com/smagafurov/fastapi-jsonrpc) - JSON-RPC server based on FastAPI.
- [Mailer](https://github.com/rclement/mailer) - Dead-simple mailer micro-service for static websites.
- [Nemo](https://github.com/harshitsinghai77/nemo-backend) - Be productive with Nemo.
- [OPAL (Open Policy Administration Layer)](https://github.com/authorizon/opal) - Real-time authorization updates on top of Open-Policy; built with FastAPI, Typer, and FastAPI WebSocket pub/sub.
- [RealWorld Example App - mongo](https://github.com/markqiu/fastapi-mongodb-realworld-example-app)
- [RealWorld Example App - postgres](https://github.com/nsidnev/fastapi-realworld-example-app)
- [redis-streams-fastapi-chat](https://github.com/leonh/redis-streams-fastapi-chat) - A simple Redis Streams backed chat app using Websockets, Asyncio and FastAPI/Starlette.
- [Sprites as a service](https://github.com/ljvmiranda921/sprites-as-a-service) - Generate your personal 8-bit avatars using Cellular Automata.
- [Slackers](https://github.com/uhavin/slackers) - Slack webhooks API.
- [TermPair](https://github.com/cs01/termpair) - View and control terminals from your browser with end-to-end encryption.
- [Universities](https://github.com/ycd/universities) - API service for obtaining information about +9600 universities worldwide.

## Sponsors

Please support this open source project by checking out our sponsors:

<a href="https://www.deta.sh/?ref=awesome-fastapi" target="_blank" title="The launchpad for all your (team's) ideas"><img src="images/deta.svg"></a>

<a href="https://testdriven.io/courses/tdd-fastapi/?ref=awesome-fastapi" target="_blank" title="Learn to build high-quality web apps with best practices"><img src="images/testdriven.svg"></a>
