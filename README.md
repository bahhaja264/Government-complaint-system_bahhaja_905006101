# Government-complaint-system_bahhaja_905006101
# PROG211 - Object-Oriented Programming
# Project: Government Citizen Complaint Management System

class Complaint:
    def __init__(self, complaint_id, citizen_name, category, description):
        self.complaint_id = complaint_id
        self.citizen_name = citizen_name
        self.category = category
        self.description = description
        self.status = "Pending"

    def display_complaint(self):
        print("\n----- COMPLAINT DETAILS -----")
        print("Complaint ID:", self.complaint_id)
        print("Citizen Name:", self.citizen_name)
        print("Category:", self.category)
        print("Description:", self.description)
        print("Status:", self.status)

    def update_status(self, new_status):
        self.status = new_status
        print("Complaint status updated successfully.")


class ComplaintManagementSystem:
    def __init__(self):
        self.complaints = []

    def add_complaint(self):
        print("\n--- Submit a Complaint ---")

        complaint_id = input("Enter complaint ID: ")
        citizen_name = input("Enter citizen name: ")
        category = input("Enter complaint category: ")
        description = input("Describe the complaint: ")

        complaint = Complaint(
            complaint_id,
            citizen_name,
            category,
            description
        )

        self.complaints.append(complaint)
        print("Complaint submitted successfully!")

    def view_complaints(self):
        if len(self.complaints) == 0:
            print("\nNo complaints have been submitted.")
        else:
            for complaint in self.complaints:
                complaint.display_complaint()

    def search_complaint(self):
        search_id = input("\nEnter the complaint ID to search: ")

        for complaint in self.complaints:
            if complaint.complaint_id == search_id:
                complaint.display_complaint()
                return

        print("Complaint not found.")

    def update_complaint_status(self):
        search_id = input("\nEnter the complaint ID: ")

        for complaint in self.complaints:
            if complaint.complaint_id == search_id:
                print("Current status:", complaint.status)

                new_status = input(
                    "Enter new status (Pending, In Progress, Resolved): "
                )

                complaint.update_status(new_status)
                return

        print("Complaint not found.")

    def run(self):
        while True:
            print("\n===================================")
            print(" GOVERNMENT COMPLAINT MANAGEMENT")
            print("===================================")
            print("1. Submit a Complaint")
            print("2. View All Complaints")
            print("3. Search for a Complaint")
            print("4. Update Complaint Status")
            print("5. Exit")

            choice = input("Choose an option (1-5): ")

            if choice == "1":
                self.add_complaint()

            elif choice == "2":
                self.view_complaints()

            elif choice == "3":
                self.search_complaint()

            elif choice == "4":
                self.update_complaint_status()

            elif choice == "5":
                print("Thank you for using the system!")
                break

            else:
                print("Invalid choice. Please enter a number from 1 to 5.")


# Main program
if __name__ == "__main__":
    system = ComplaintManagementSystem()
    system.run()
