# Analyze with Codecov

Upload coverage reports to Codecov. Leverages the official [codecov-action](https://github.com/codecov/codecov-action) pre-configured specifically for the majority.

> This action is part of the Codebelt ecosystem and ensures a consistent way of: 
> 
> - Defining your CI/CD pipeline 
> - Structuring your repository
> - Keeping your codebase small and feasible
> - Writing clean and maintainable code
> - Deploying your code to different environments
> - Automating as much as possible
>
> A paved path to excel as a DevSecOps Engineer.

## Usage

To use this action in your GitHub repository, you can follow these steps:

```yaml
uses: codebeltnet/codecov-scan@main
```

### Inputs

```yaml
with:
  # The Codecov generated token.
  token:
  # The fully qualified name of the repository.
  repository:
  # The path to the Codecov Yaml file.
  configuration: '.codecov/codecov.yml'
```

### Outputs

This action has no outputs.

## Examples

### Push coverage reports to Codecov

```yaml
steps:
  - name: Run CodeCov Analysis
    uses: codebeltnet/codecov-scan@main
    with:
      token: ${{ secrets.CODECOV_TOKEN }}
      repository: codebeltnet/savvyio
```

## Contributing to Analyze with Codecov

Contributions are welcome! 
Feel free to submit issues, feature requests, or pull requests to help improve this action.

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
