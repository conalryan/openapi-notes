# hello-world

`swagger-codegen generate -i ../hello_world.yaml -l jaxrs-cxf -o out -c config.json`

`swagger-codegen config-help -l jaxrs-cxf`

e.g.
`
CONFIG OPTIONS
	sortParamsByRequiredFlag
	    Sort method arguments to place required parameters before optional parameters. (Default: true)

	ensureUniqueParams
	    Whether to ensure parameter names are unique in an operation (rename parameters that are not). (Default: true)

	allowUnicodeIdentifiers
	    boolean, toggles whether unicode identifiers are allowed in names or not, default is false (Default: false)

	modelPackage
	    package for generated models

	apiPackage
	    package for generated api classes

	invokerPackage
	    root package for generated code

	groupId
	    groupId in generated pom.xml

	artifactId
	    artifactId in generated pom.xml

	artifactVersion
	    artifact version in generated pom.xml

	artifactUrl
	    artifact URL in generated pom.xml

	artifactDescription
	    artifact description in generated pom.xml

	scmConnection
	    SCM connection in generated pom.xml

	scmDeveloperConnection
	    SCM developer connection in generated pom.xml

	scmUrl
	    SCM URL in generated pom.xml

	developerName
	    developer name in generated pom.xml

	developerEmail
	    developer email in generated pom.xml

	developerOrganization
	    developer organization in generated pom.xml

	developerOrganizationUrl
	    developer organization URL in generated pom.xml

	licenseName
	    The name of the license

	licenseUrl
	    The URL of the license

	sourceFolder
	    source folder for generated code

	localVariablePrefix
	    prefix for generated code members and local variables

	serializableModel
	    boolean - toggle "implements Serializable" for generated models (Default: false)

	bigDecimalAsString
	    Treat BigDecimal values as Strings to avoid precision loss. (Default: false)

	fullJavaUtil
	    whether to use fully qualified name for classes under java.util. This option only works for Java API client (Default: false)

	hideGenerationTimestamp
	    Hides the generation timestamp when files are generated.

	withXml
	    whether to include support for application/xml content type and include XML annotations in the model (works with libraries that provide support for JSON and XML) (Default: false)

	useOas2
	    use OpenAPI v2.0 (Swagger 1.5.x) (Default: false)

	dateLibrary
	    Option. Date library to use
	        joda - Joda (for legacy app only)
	        legacy - Legacy java.util.Date (if you really have a good reason not to use threetenbp
	        java8-localdatetime - Java 8 using LocalDateTime (for legacy app only)
	        java8 - Java 8 native JSR310 (preferred for jdk 1.8+) - note: this also sets "java8" to true
	        threetenbp - Backport of JSR310 (preferred for jdk < 1.8)

	java8
	    Option. Use Java8 classes instead of third party equivalents
	        true - Use Java 8 classes such as Base64
	        false - Various third party libraries as needed

	implFolder
	    folder for generated implementation code

	title
	    a title describing the application

	useBeanValidation
	    Use BeanValidation API annotations (Default: false)

	serverPort
	    The port on which the server should be started

	generateSpringApplication
	    Generate Spring application (Default: false)

	useSpringAnnotationConfig
	    Use Spring Annotation Config (Default: false)

	useSwaggerFeature
	    Use Swagger Feature (Default: false)

	useSwaggerUI
	    Use Swagger UI (Default: false)

	useWadlFeature
	    Use WADL Feature (Default: false)

	useMultipartFeature
	    Use Multipart Feature (Default: false)

	useGzipFeature
	    Use Gzip Feature (Default: false)

	useGzipFeatureForTests
	    Use Gzip Feature for tests (Default: false)

	useBeanValidationFeature
	    Use BeanValidation Feature (Default: false)

	useLoggingFeature
	    Use Logging Feature (Default: false)

	useLoggingFeatureForTests
	    Use Logging Feature for tests (Default: false)

	generateSpringBootApplication
	    Generate Spring Boot application (Default: false)

	generateJbossDeploymentDescriptor
	    Generate Jboss Deployment Descriptor (Default: false)

	addConsumesProducesJson
	    Add @Consumes/@Produces Json to API interface (Default: false)

	useAnnotatedBasePath
	    Use @Path annotations for basePath (Default: false)

	generateNonSpringApplication
	    Generate non-Spring application (Default: false)

	useGenericResponse
	    Use generic response (Default: false)
`