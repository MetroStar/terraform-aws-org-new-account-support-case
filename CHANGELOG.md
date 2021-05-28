## terraform-aws-org-new-account-iam-role Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/) and this project adheres to [Semantic Versioning](http://semver.org/).

### 0.2.1

**Commit Delta**: [Change from 0.2.0 release](https://github.com/plus3it/terraform-aws-org-new-account-support-case/compare/0.2.0...0.2.1)

**Released**: 2021.05.28

**Summary**:

*   Corrects lambda policy to allow support:DescribeCases.

### 0.2.0

**Commit Delta**: [Change from 0.1.1 release](https://github.com/plus3it/terraform-aws-org-new-account-support-case/compare/0.1.1...0.2.0)

**Released**: 2021.04.29

**Summary**:

*   Revise integration test so it can successfully complete the lambda
    invocation.

### 0.1.1

**Commit Delta**: [Change from 0.1.0 release](https://github.com/plus3it/terraform-aws-org-new-account-support-case/compare/0.1.0...0.1.1)

**Released**: 2021.04.28

**Summary**:

*   Use a different docker name for the integration tests.

### 0.1.0
    
**Commit Delta**: N/A

**Released**: 2021.04.09

**Summary**:
        
*   Add two more environment variables for Lambda:  SUBJECT and
    COMMUNICATION_BODY.  Permit the variable 'account_id' to be used within 
    the text of those two new environment variables.
*   Updated the Terraform configuration to add the policy document to
    provide the Lambda with permissions for 
    organizations:DescribeCreateAccountStatus.
*   Modified the unit tests to replace the monkeypatched function for
    get_account_id with a call to moto organizations service to set up an 
    obtain an organizations account ID.

### 0.0.0

**Commit Delta**: N/A

**Released**: 2021.03.30

**Summary**:

*   Initial release!
