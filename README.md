Linux File Permission Analysis
Objective

Identify overly permissive Linux file permissions.

Tools

Browser-based Linux terminal, chmod, and ls -l.

Permission Analysis
777: Owner, group, and others can read, write, and execute. This is excessive for ordinary files.
755: Owner can read, write, and execute; group and others can read and execute.
644: Owner can read and write; group and others can read.
Findings

The sample files initially showed overly permissive access. Permissions were changed and verified using ls -l.

Remediation

Used chmod to demonstrate safer permissions following the principle of least privilege.

Evidence

See permission-evidence.png for terminal evidence.

Rollback

See rollback.txt for commands to restore the documented final permissions.

Conclusion

Excessive permissions can allow unauthorized modification or execution. Appropriate permissions reduce security risks.
